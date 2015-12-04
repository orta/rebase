---
layout: post
title: Why won't my CocoaPods Page Expand?
uuid: EF44345-82101-29BAD-E4324-sdd
---

The CocoaPods Website is pretty complex, but it's not a black box. Occasionally I see questions asking about what is going on with their pods. So lets look at ways in which you can debug a library that isn't expanding on CocoaPods.org.

We'll go through an example I just looked at, [SCConfiguration](http://cocoapods.org/pods/SCConfiguration). The end result is that we want to be able to show the Pod page that looks like this:

<img src="/rebase/assets/images/sccconfig-pod-page.png" alt="Sccconfig Pod Page" width="100%">

There are two places to start looking at the problem:

* *CocoaDocs*

  First up, load up the expected URL in CocoaDocs. The URL will look like [http://cocoadocs.org/docsets/[pod]/](http://cocoadocs.org/docsets/SCConfiguration/) if you get a 404 then that means CocoaDocs could not parse your library. 
  As a rule of thumb, CocoaDocs is stable and works. 
  
  The most common problem with generating documentation is that your library crashes either [appledoc](http://appledoc.gentlebytes.com/appledoc/) or [jazzy](https://github.com/realm/jazzy). This tends to happen when you use bleeding edge features in betas of Xcode.
  
  The 404 page offers a button to request that CocoaDocs takes a second look at running your library, the URL for this is [http://api.cocoadocs.org:4567/redeploy/[pod]/latest](nope://hah)
  
  CocoaDocs also offer a way to see errors from CocoaDocs related to a pod. The URL for this [http://api.cocoadocs.org:4567/error/[Podname]/[Version]](http://api.cocoadocs.org:4567/error/SCConfiguration/1.0.0). You'll get a 404 if there's no logged errors.
  
  You can find out a bit more about CocoaDocs in the [Pod Authors README](http://cocoadocs.org/readme/).

* *metrics.cocoapods.org*

  Once CocoaDocs has done it's work, it sends a bunch of useful metadata to the CocoaPods database. The best way to see what's going on under the hood here is to look at the metrics for your pod. There are three exposed sections in the database: github, cocoadocs, stats. In order to show the Pod page the `cocoadocs` section of your metrics has to exist.
  
  The url for the pod metrics is [http://metrics.cocoapods.org/api/v1/pods/[pod]](http://metrics.cocoapods.org/api/v1/pods/SCConfiguration). In this case you can see cocoadocs data, so the pod page will show.
  
### So the metrics shows stats and there is documentation on CocoaDocs, but not on the CocoaPods Search

Check your pod page, jump specifically to the URL: [http://cocoapods.org/pods/[pod]](http://cocoapods.org/pods/SCConfiguration), if that works then everything is OK. The search database is asyncronous with respect to changes in underlying data of the database. It could take an hour or two for the fix to propogate back to search.

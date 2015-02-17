---
layout: post
title: A Story on OSS Management
uuid: EF44345-8210D-49BD-E4324-sdd
---

> “The bottleneck is never code or creativity; it's lack of clarity.”

<p class="source"> Excerpt From: Scott Berkun. “<a href="http://www.amazon.com/The-Year-Without-Pants-WordPress-com/dp/1118660633">The Year Without Pants.</a>”</p>

Projects drift. Maintainers move on. New languages come, and the world feels a bit brighter somewhere else. The grass is greener there. I've got a new job. I have a kid. There are a million reasons for a project maintainer to move on.

In theory a high profile project won't perish. People use it. However, high profile projects still need continual work and for contributors to feel that there's value in contributing.

I’d like to give an example, `Specta` / `Expecta` is a project that has had many contributors over the past 5 years. There’s always been one main contributor, [Pete J Kim][1]. He works on it in spurts roughly twice a year. He’s done a brilliant job of getting it to be a staple part of the community, and last year I opted to make it the default for creating a new pod via `pod lib create`.

The project was in a weird place last month, before Swift came out the plan was to do some major restructuring, and add some features for the next release. This work ended up getting mixed in with Xcode 6 compatability and Swift support. In July 2014, at Xcode 6’s launch it looked like everyone building libraries had some work to do. By Febuary 2015 there still wasn’t a new public release of Specta. In early January ago I ended up giving up on hoping for a [new version][2] and was willing to set a bad example in every new pod because of this.

This is not to say that I blame Pete for anything, he has his own priorities, as do the rest of the Specta organization. However, I was relying on it. 

So I did what anyone should do. I told my colleagues in [Artsy mobile][3] that my progress was going to be a bit slower than normal this week and that I was going to devote some time to Specta and Expecta. I spent some time going through what Pull Requests were open, what issues had already been fixed and created a [1.0 manifesto][4].

This was a clean issue stating exactly what I thought needed doing to get Specta solid. It explained my reasoning and showed what I thought needed to be done in order to get to that point.

I created the issue, then tweeted Pete, then gave it another day and emailed. He replied that this was awesome and gave me push access the next day. This was validation. 

In creating the 1.0 issue I started to awaken some older contributors to rebase old Pull Requests, and to start picking off parts of the issue that I hadn’t done. I triaged all the issues eventually closing over half of the issues, creating test projects to verify if something had been fixed. Merged Pull Requests that had been sitting for months. Updated the documentation and the README with modern images. In the end I barely [contributed any code][5]. In fact, a [new contributor][6], Pawel Dudek, appeared to help out with a lot of the programing. After giving it my spare project time for day or two it was in a great position and I gave it a public release.

Specta has a sibling project Expecta, so I started going through the same process over there. Writing up a [1.0 Manifesto][7] so that people could give feedback if they disagreed with the vision. _Just writing it can be enough_. The fact that there was a plan got [Tony Arnold][8] to do a huge amount of refacoring and cleanup. Given his understanding of the tool itself, he got a huge amount done over the course of [two days][9]. Enough that it ticked almost all of my check boxes. With it wrapped up, I helped test it out and get a release out.

Projects need someone with a vision and a path, if you’re interested in contributing to a large project here’s some concrete steps that have worked for me in CocoaPods, and in Specta.

* Be a user of the project.
* Start by triaging issues to see what the common problems are, closing duplicates and interlinking issues as much as possible. Even if you don’t have the ability to close issues, writing “dupe of #11” is really useful.
* Offer a vision, and be willing to be the person to do it.
* Ask for more power. In the open source world, power is granted easily. Mentoring isn’t easy, but they will nealry always be willing to [bet on you][10].
* Use backchannels to communicate if necessary.
* Actually do the work you said you would. [Deflect][11] [the][12] [praise][13], take ownership of [problems][14].

Improve the community by improving existing tools instead of re-inventing wheels, and make a name for yourself by working on hard things.


[1]:	https://github.com/petejkim
[2]:	https://github.com/CocoaPods/pod-template/commit/4f97d1bcc9a529639763a5b009426da1f4d9c7c1
[3]:	https://github.com/artsy/mobile/
[4]:	https://github.com/specta/specta/issues/125
[5]:	https://github.com/specta/specta/commits?author=orta
[6]:	https://github.com/specta/specta/commits/master?author=paweldudek
[7]:	https://github.com/specta/expecta/issues/127
[8]:	http://tonyarnold.com
[9]:	https://github.com/specta/expecta/commits/master?author=tonyarnold
[10]:	http://blog.cocoapods.org/starting-open-source/
[11]:	https://twitter.com/orta/status/565281653745254401
[12]:	https://twitter.com/orta/status/566240952839598080
[13]:	https://github.com/specta/specta/issues/125#issuecomment-73878558
[14]:	https://github.com/specta/specta/issues/127#issuecomment-73786443
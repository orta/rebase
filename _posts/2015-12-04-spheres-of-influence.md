---
layout: post
title: Spheres of Influence
uuid: EF41545-82101-29BAD-E4324-sdd
---

We all want to make an impact. Somehow.

My girlfriend is a Podiatrist, she makes a direct impact on everyone she helps. The people who she helps out can come away from that interaction with a noticeable positive difference in their life. She can make an impact that lasts for months in span of 15 minutes.

Her sphere of influence however, is small. A direct impact on a small number of people. In a discrete area.

When I started contributing to the Open Source community, my impact was pretty small. I started by shipping all my apps as OSS by default in my teens. No one read the code, it also pre-dated pull requests. So I got no feedback.

Undeterred, I got better. The tools got better.

I initially had to fight to write code at my job, I was working as a phone support person, but there were so many places that automation could improve my flow. I pitched every week that I could work on _a thing_. Eventually, 2 weeks before I left the company, I switched to working on it full time. I made it open source by default. It's still [around](https://github.com/orta/virtualapps).

It had a positive impact on the people on my team, and potentially the ~100 people who would need to use it.

When I worked at a programming camp, I taught iOS to budding developers. Rather than make course material, I built OSS infrastructure and libraries to help reduce the amount they needed to learn to get something on screen. The most notable example is  [WibbleQuest](http://orta.io/WibbleQuest/). I taught more than 100 kids using these OSS tools.

Once that finished, I joined Artsy. Artsy wasn't an OSS powerhouse, though it had the right mindset, it was at ~15 people trying to ship an idea. There was no mobile team, just a development team. My impact correlated to the amount of code I could ship.

In my first year, I took over a [single gem](https://rubygems.org/gems/pt), and started a small [analytics library](https://cocoapods.org/pods/ARAnalytics). I was impacting thousands of developers a little bit.

In my second year at Artsy, I started running the [CocoaPods Specs](https://github.com/CocoaPods/Specs/commits/master?author=orta&page=25) repo. This meant interacting with people [directly](https://github.com/CocoaPods/Specs/pull/565), [and](https://github.com/CocoaPods/Specs/pull/576) [trying](https://github.com/CocoaPods/Specs/pull/577) [to](https://github.com/CocoaPods/Specs/pull/612) [help](https://github.com/CocoaPods/Specs/pull/601) [make](https://github.com/CocoaPods/Specs/pull/1051) [a](https://github.com/CocoaPods/Specs/pull/1070) [better](https://github.com/CocoaPods/Specs/pull/1033) [community](https://github.com/CocoaPods/Specs/pull/1363). No one asked me to help out, it just took too long to get PRs in when I submitted one.

Half a year of that, and I was comfortable fixing a harder problem with the community. I [started working](https://github.com/CocoaPods/cocoadocs.org/commit/93e9896b04f79eb09be28a9056671b1d23f3143d) on CocoaDocs. I didn't tell people in CocoaPods that I was doing it, I didn't announce my intentions. I just shipped it, and announced it. The validation came a few months later, as more [libraries](https://github.com/AFNetworking/AFNetworking/commit/22ba1c863648f4d50b673319bac3506a5fc9adde) started to support it as their main source of documentation. At this point there were only about 1,500 CocoaPods.

In my third year of Artsy, we created the mobile team. I used my reputation from CocoaDocs to start landing [conference talks around the world](http://orta.io/#speaking). I did this because I could visit my girlfriend in the UK, and because I wanted people to work with. [It worked](https://ashfurrow.com/blog/new-job/).

Having a mobile team meant being able to create a culture. At first we were indistinguishable from every dev team in artsy. It took maybe a year to decide what the mobile team even was.

With CocoaDocs stable, I started work on a much harder project: [redesigning CocoaPods](http://blog.cocoapods.org/redesign/). This project touched every part of the public representation of CocoaPods. It involved working closely with a lot of people, on a project they cared about. We made the site easier to use, vastly improved documentation  and offered clear communication channels. We were seeing about 1,000 people a day on the CocoaPods site when we switched the design.

In my fourth year of Artsy, I cemented what it means to be a mobile engineer at Artsy. Probably, for the rest of Artsy's lifetime. With help from Ash, we made every application open source, and established a culture of open source by default from then on. I got to a point where I didn't need to do so much programming, as I wanted to work on different problems. We hired some more awesome people, and now our impact isn't just within Artsy, but on the entire Cocoa community.

Within CocoaPods I helped us make the [transition](http://blog.cocoapods.org/The-captain-leaves-the-bridge) from small group of hackers, to a [considerable team of people](https://cocoapods.org/about) and voices. CocoaPods became the default integration methods for the majority of SDK providers, and it is assumed now that every library supports CocoaPods.

In the process, I've used CocoaPods' ubiquity to improve the code quality for the tens of thousands of libraries, by offering analytics, showing ways to improve libraries programmatically and adding extra features for libraries that conform to general standards.

We now get 100,000 unique people visiting the CocoaPods website looking for ways to improve their apps. In the last 3 months there were 30 million pods integrated by CocoaPods.

At the end of this year, I've been working with [@alloy](https://github.com/alloy) on the CocoaPods app. I think it will become the default way for most people to work with libraries in their apps, for a long time. It lowers the barrier to entry even more, and makes life considerably easier for beginner -> informed developers.

Yesterday, Apple announced Swift as open source, and along came a [Package Manager](https://github.com/apple/swift-package-manager/). The Package Manager is made by people from the CocoaPods community, they know the positives and negatives from our decisions. Within 2-3 years, the Swift Package Manager will be solid and the default for all new libraries.

I started, and continue working on CocoaPods because it was a project that allowed for personal growth, that had a space that I had the skills to work on. I could work on projects that have a large impact on communities that I care about. Dependency Management itself has never been a particularly interesting project for me, but working at the level of an entire community does. We have to make hard decisions.

My sphere of influence has never been greater. However, that sphere is mostly developers. Sure, they create things that other use. It's a pretty safe bet that the iPhone of everyone I meet here in NYC has code that CocoaPods has touched. However, I want to keep increasing that sphere, working on harder problems. Touching more people in meaningful ways.

I feel like the CocoaPods App is probably going to be my last major project at CocoaPods. I have a lot to maintain, so I'm not going anywhere, but having Apple in the space definitely makes it easier to start work on the projects I've been [talking](https://twitter.com/orta/status/634060944528814081) about doing for the last year or two.

There's still a lot of really interesting work to do in the Cocoa community, but maybe it's better to recognise that it's not a singular community anymore. It's going to be a weird transition from "Cocoa community" to "Swift community" + "Cocoa communuty".

I've been feeling the tension from it the last year. It's why I started talking about everyone raising the bar on [being nice](https://twitter.com/lascorbe/status/608757355845570560).

In my fifth year of Artsy, I expect to be doubling the mobile team. I want to get more people into a position where they feel like how Ash talks about in his post on [Building His Career](https://ashfurrow.com/blog/building-my-career/). I want to program even less. I want the mobile team to have exponentially more users on their apps.

I want my free time to have even more of an impact on the world than it does now. To do that, I need to stop new work on developer tools. There are other non-trivial projects that I should devote my time to.

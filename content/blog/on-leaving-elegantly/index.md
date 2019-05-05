---
title: "How to leave elegantly"
date: "2019-04-15"
---

I've been at Artsy now for seven and a half years, and next I'm heading out to go work on the [TypeScript
programming language][typescript] at Microsoft. This wasn't a surprise to my close collaborators, but likely was a
surprise for the rest of the company and externally.

I want to talk through how I tried to prepare the company for my departure by de-coupling myself from owning
important code and processes, and by setting up many people to continue to push Artsy's engineering culture
forward.

## My Role at Artsy

I'm an Engineer who has been at Artsy since close to the beginning. Artsy has a few pretty complex businesses, and
I've touched most of them in some way. I've always aimed to ensure that engineering in Artsy doesn't feel
disconnected to the rest of the company, and I spend quite a lot of time talking externally (I account for over a
quarter of the blog posts on this site for example) about our work.

Strictly speaking, none (and all) of these are in my job role which has evolved over the years to a kind of
architect-ish role of knowing [a lot about everything][shallow] and mainly assisting people work on those, plus
making infrastructure which allow [others][danger] [to][peril] [do][docs] [more][stitching] with less. Which makes
leaving leaving a bit tricky, I might not own a lot of things, but a lot of my value has been in the soft-skills
in-between.

<!--
require "yaml"
YAML_FRONT_MATTER_REGEXP = /\A(---\s*\n.*?\n?)^((---|\.\.\.)\s*$\n?)/m

ortas_posts = Dir.glob("*").select { |f|
  content = File.read(f)
  found = false
  if content =~ YAML_FRONT_MATTER_REGEXP
    data, content = YAML.load($1), Regexp.last_match.post_match
    if data["author"] == "orta" || data["author"].include?("orta")
      found = true
    end
    puts data
  end
  found
}

ortas_posts.length
 -->

## On Leaving

Reasonably speaking, I'm a pretty open book. For the last 9 years I have publicly written a pretty personal annual
write-up of the ups and downs of my life, my relationships to Open Source and Artsy. They're available on my
website [orta.io][]. Almost all the engineers who I spoke to about leaving said that it fit with my last write-up.

I didn't want to leave until I had deprecated myself.

Regardless, as engineers this should be a constant goal. Deprecating yourself via process, automation or delegation
gives you more space to work on upcoming problems. In any company there are always new problems and keeping
yourself nimble will give you a better chance at tackling them. Being indispensible at one thing is only valuable
for the current status quo, and tech moves fast.

Throughout my career at Artsy I've changed roles regularly as Artsy has grown and changed. When Artsy needed an iOS
engineering team, I became a manager, then when we moved to React Native and de-siloed the team - we didn't need
that anymore and I went back to being an individual contributor and someone who made more sense took those
responsibilities. This is one of my favourite things about start-ups, they change often. If you're creative, put
the time in and are open to being uncomfortable occasionally then there are all sorts of experiences ahead.

In 2018 what Artsy needed was someone to look holistically at the Engineering team from the inside. I picked up a
chunk of soft-skill responsibilities in order to ensure Artsy's Engineering was in tip-top shape, working on
everything from hiring to team cohesion.

# Rebasing Responsibilities

7.5 years is a long time! I've had to use quite a few techniques to distribute responsibilities over time, however
leaving a company really does inspire you to get through them quicker. Here's some of the tactics I've used over
the years, and how tey were angled to promote growth within the rest of the Artsy Engineering team.

### Split your roles into smaller pieces, and with a tighter and more obvious scope

A good example of splitting roles came from owning all of the front-end practice at Artsy. Effectively making sure
we had common goals and were sharing our best ideas across web and mobile. I realised that there were people
interested in owning subsets of the global front-end practice and if I split it into web and iOS they would have
the opportunity to give each platform more focus.

### Build process changing tools, use them yourself to set an example, then lay off the gas

Throughout 2018 I spent a lot of time improving Artsy's engineering culture, mostly [using RFCs][rfcs]. In 2019 I
stopped creating new RFCs and only worked on RFCs as a co-signer which was owned by someone else.

In 2019, we started to see a much more diverse set of engineers writing new RFCs which give the team access to a
lot of new and interesting ideas and the RFC process has never been as active. I'm really proud of the work others
are doing with this process.

### Create working groups to allow many people to work on a problem collectively

I have always been a good fallback for ownership of projects which fall between the gaps between teams. For
example, I own our company dashboard and our internal team navigator. While these projects are important but they
would really need an engineering focused on internal tools to get changes added to a roadmap. Given Artsy's size
today, that's not likely to happen.

To try mitigate a single point of failure, I created one of the first engineering working groups in Artsy. With the
focus being an intersection between our workplace team and engineering to keep track of any high impact easy wins
for internal culture. Anyone was welcome to join from engineering, and over time new folks started showing up and
helping.

Since then working groups have popped up everywhere in Artsy, driven by engineers and product managers depending on
needs. I've tried to take a back-seat in these and really enjoyed being a contributor.

### Mentor potential successors

I don't expect anyone to directly replace me, but this is a common tactic when leaving, but when someone shows any
related interest - dive in and offer anything to help them. Mid 2018 I opened up some extra 1 on 1 spaces in my
calendar (by consolidating them all to one single day every 2 weeks) and specifically targeted folks who I think
would do a good job at taking some of responsibilities over time.

That said, we [specifically targeted][twitr] getting at least one person who would care about tooling in a way that
echoes my opinions when hiring, and that worked out well.

### Document everything

If you do enough [defensive OSS][def-oss], you learn the value of the up-front cost of docs vs long term questions
from people. Even internally I try to write docs for someone's question rather than answering directly. This
pattern of externalizing answers inspires a hefty amount of my blog posts on the Artsy blog, while writing this way
can be slower, that answer can be more thoughtful and better articulated.

I took the time to focus a lot of our documentation across all of engineering into two centralized places (one in
the open (default) one private (fallback)) which dramatically increased the number contributors to team
documentation across the company.

In terms of code documentation, I've been sneaking documentation updates to as many projects as I can. For example,
on a project with a pretty low [number of contributors][energy-contrib] I added documentation specifically aimed at
providing coverage of [features per-screen][energy-map].

### Cleaning the backlog

When there's a time limit, it really helps you focus on getting some of those long running PRs in. I shipped a
feature that I had been working [on and off for 5 years][folio-album-sync] last month.

I'm currently going through a process of hitting all my backlog posts for the Artsy blog, as well as trying to
cement the reasoning for things I think are worth keeping around. Ultimately though, it's up to the rest of the
engineering team to decide whether a cultural pattern is worth keeping or a project is worth maintaining.

## Give your company the best chance to make a competing offer

I wanted to give Artsy the best chance to compete with an offer like the one from TypeScript. One of the best
strategies for this came up when speaking with Samuel, our VP of Engineering. He recommended that I imagine that I
didn't work at Artsy, and figure out the job role which would be the most attractive to me.

We explored this idea and created a really compelling job role which fit for both Artsy and me. It was a refreshing
take what I've enjoyed from my time with Artsy, and things I'm interested in doing in the future. It ended up like
this:

```
## Head of OSS at Artsy

Roughly:
- Make Artsy OSS Awesome
- Help ship big things in parallel work streams with product
- Make it fun and full of growth to be at Artsy

Goal: Ensure Artsy OSS thrives.
Aim: Externally cement that Artsy's tech credentials are solid, and provide external stimulus for Art-world folks to work with us

- ~ 4–5 tech conference talks a year
- ~ 1-2 arts conferences/fairs/panels a year
- ~ 12 solo blog posts per year

- Also:
  - Ensuring every major tech launch has a write-up (e.g. New Selling Options, Show Guide )
  - Ensuring all libraries we OSS are documented, tested, and usable outside of Artsy
  - Helping internal engineers from those teams write public talks about the launches and what we had to build

Goal: Help ship longer-term perspective which runs parallel to the roadmap
Aim: Help make the team make less short-term choices

Work with one other person to ship some of the things Artsy has found difficult to work due to
roadmap tradeoffs, but that we feel needs to get done eventually:

- Explore building standalone services for model domains (artworks/partners/shows etc)
- Work on how we can we standardize admin UIs
- Provide a technical roadmap, and own what it takes to ship an android app
- Own the third party API (handle legal rights, own docs + evolution)
- Consolidate JS tooling into something which sits above express/rails/react-native

These are projects we've regularly said "want to do that, but it'd block shipping X or Y", where
as a team we consciously decide to continue a larger technical debt in favour of shipping something.

Goal: Maintain and improve Artsy's culture
Aim: Make Artsy feel like an awesome place to work

Run events:

- Demo Days
- Lunch & Learns
- Provide more support to initiatives like Artsy Learns to Code
- Explore

Cohesion:
- Focus on 1on1s with product + designers to help them grow
- Run workshops for all of Artsy to help raise technical awareness
```

Sounds like a great fit right? This role some of the things I was already doing on the side, and moves them to be
forefront as well as trying to work well with the rest of the company and ship some big things.

In the end, after giving Artsy the chance to make the best offer, I had to make a decision. I'm inspired by the
scale of impact when working on TypeScript. Being able to help shape and evolve the language is such a compelling
offer that I chose Microsoft. Artsy still had a lot to offer, but for me it was time to try something new.

I think the idea of "what is an optimal offer for your current company" is a pretty good pattern for anyone who has
a long tenure at a company to explore. It gives your current company a way to show off it's best attributes and you
already have the existing relationships to make it work.

## Letting People Know

I spent a considerable amount of time thinking about this. I'm not sure there's a perfect way, but I can at least
talk to what I did. I had a few aims: tell people individually then in groups, strive for as natural a setting as
possible and make it easy to know who knows so far.

I structured my timeline to look roughly like:

- Inform my manager + direct collaborators when I was taking informationals (maybe 2-3 months prior to signing)
- 1st week after signing - all collaborators, this came to roughly 120 people
- 2nd week, Monday - ensure all dev knows by announcing it at our team stand-up
- 2nd week, Tuesday - email most of the team
- 2nd week, Wednesday - let the internet know

For the few days, while it was hard to keep track of who know, I used a private slack channel (called
[#oort-cloud][oort-img]) where I added people as I told them, it turned into a pretty fun support-group channel for
light-hearted jabs and interesting discussions.

A week and a few days is quite a while to keep the announcement somewhat secretive, but in general it held. This
gave me the chance to answer a lot of questions personally. While I came home drained every night, I feel like I
did the right thing for the people I'm leaving.

## Final Days

When I considered what the right thing to do with my final days, I felt that some of the best value I can give to
Artsy is in providing historical context. That's why I've been shipping so many blog posts in 2019. I'd like to try
dig deeper and pull out some interesting stories from other oldbies at the company. I'm also going to improve our
alumni network, so it's easy to keep in touch with Artsy folks because I'm going to miss a lot of them.

I got a lot of recommendations to take time off between jobs, considering I have been focusing my thinking around
Artsy for a very long time then finding a mental space where you can felt empty sounded compelling.

[orta.io]: https://orta.io
[rfcs]: /blog/2019/04/11/on-an-rfcs-process/
[twitr]: https://twitter.com/orta/status/954085934781358081
[def-oss]: /blog/2016/07/03/handling-big-projects/#Issues
[energy-contrib]: https://github.com/artsy/energy/graphs/contributors
[energy-map]: https://github.com/artsy/energy/blob/master/docs/feature_map.md
[folio-album-sync]: https://github.com/artsy/energy/pull/189
[danger]: https://artsy.github.io/blog/2017/06/30/danger-one-oh-again/
[peril]: https://artsy.github.io/blog/2017/09/04/Introducing-Peril/
[shallow]: https://artsy.github.io/blog/2018/08/10/On-Context-Switching/
[docs]: https://artsy.github.io/blog/2018/08/21/OSS-by-Default-Docs/
[stitch]: https://artsy.github.io/blog/2018/12/11/GraphQL-Stitching/
[oort]: https://en.wikipedia.org/wiki/Oort_cloud
[typescript]: https://www.typescriptlang.org
[oort-img]: /images/on-leaving/oort-cloud.png

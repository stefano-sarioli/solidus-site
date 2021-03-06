---
title: Forking Spree - Solidus Two Years Later
date: 2017-08-30
tags: Spree, Solidus, forked
author: Solidus Core Team
---

[Since forking Spree](https://solidus.io/blog/2015/10/28/future-of-spree.html) we’ve been so busy putting together our [5329 artisanally-crafted solidus core commits](https://github.com/solidusio/solidus/graphs/contributors), we often forget to stick our head out of our git logs and talk about where we are and where we’re going. During one of the [SolidusConf 2017](https://youtu.be/TSbUnRPbeK0?list=PLQNruX2oZ7ZFQrXZ2WmRtCB5Bi5wjCIeB) keynotes, the Solidus core team made a commitment to more frequently discuss the state and direction of the Solidus project. Before we get into where we’re going, we thought a good place to start is examining how far we’ve come in our two years since forking.

Last April (2016) Stembolt wrote about [why we’d forked Spree and started Solidus](https://stembolt.com/blog/why-we-forked-spree-and-started-solidus/). Since that post was written we’ve had two successful SolidusConfs ([Toronto, Canada](http://conf2016.solidus.io/) and [London, England](http://conf2017.solidus.io/)), seen adoption skyrocket, and watched our community grow and thrive. Less visibly, through that time the Solidus Core team and the community at large has had its heads-down working on improving the technical side of the Solidus ecosystem.

While there are many ways to judge the strength and health of a project, a good place to start is to reflect on the goals we set for ourselves when we forked Spree.

# The Original Goals of Solidus

In April 2015 we held the first SolidusConf, a quiet retreat in the mountains of Whistler, BC. We hunkered down with the goal of building a roadmap for Solidus, independent from the Spree project.

We wanted to fix what we saw as wrong with the project and plan for its future. It was important to vocalize and cement where we wanted the platform to go and needed concrete goals we could measure ourselves against.

The conference came up with six points we knew would make the project a success. Once our fork was public, they were posted on the homepage of solidus.io as signposts for other developers that shared our goals and concerns.

![The original Solidus goals](/blog/2017/08/30/forking-spree-solidus-two-years-later/original-solidus-goals.png "The original Solidus goals")

# Reviewing Solidus’ Original Goals

## We’ve Earned the Trust of Open Source Developers
We’ve been uncompromising in our standard of development. We give a broken test suite our highest priority. Every PR is reviewed by at least two seasoned Solidus core members before it is merged. The improvements we’ve made to our test infrastructure and general reliability have directly translated into improvements in the tests and reliability of every store that uses Solidus.

## Our API is Stable
We’ve been diligent about deprecating outdated API’s, while continuing to support them through numerous releases to give our users as much time as possible to adapt to the change. The HTTP API has been almost completely backwards compatible since we started, giving stores a guaranteed point of stability when using Solidus.

## More Extension Points Means Easier Customizations
While increasing extensibility will be a never-ending series of improvements to the codebase, we’ve come a long way since we forked from Spree. We’ve established many extendable interfaces into complex aspects of the system, allowing stores to easily customize their needs in future-supported ways. The [flexible pricing system](https://github.com/solidusio/solidus/commit/92048533ffbf939386cd0a593a8cb4619cf7eae3) by [Martin](https://github.com/mamhoff) has been an excellent example of how we’ve made seemingly-simple changes that have drastic impacts in our usability and extensibility.

## We’re Proud of Our Secure Platform
It wasn’t long after we published our goals that administration roles were audited and extended in Solidus, giving stores the ability to control the actions of their admins. For the first time we could grant people access to areas of the backend without wondering if they were going to accidentally take down their store. We fixed many inherited security vulnerabilities, continue to audit our own code, and are proud that with our dilligence we haven't had a single critical vulnerability introduced since we forked. There's more work to do here, especially in making these security features more widely used.

## Upgrading is Easier Than Ever Before
The most common feedback we received during SolidusConf London was from stores that were finally able to upgrade without running into countless roadblocks and headaches. What has taken stores months to accomplish can now be done in an afternoon. Judging from the enthusiasm in the discussions of all the steps we’ve taken, this is the one that has made the largest positive impact to Solidus users.

## We’re Still Passionate About the Project
With the exception of [John Hawthorn](https://github.com/jhawthorn) – who maintains the open source side full time – all the core members are still involved in the day-to-day development and operation of Solidus stores.

# We Were on the Radar
Six months after we quietly posted our goals, and four months after the release of Solidus 1.0, Spree Commerce announced they were acquired and would no longer maintain the Spree platform. The people we respected most in the community had known about our fork and appreciated our goals and the direction we were headed. A notice was added to the Spree repo directing traffic to Solidus.

![Notice that Spree is no longer maintained posted by Radar in November 2015](/blog/2017/08/30/forking-spree-solidus-two-years-later/add-notice-spree-is-no-longer-maintained.png "Notice that Spree is no longer maintained")

We took this validation and put our heads down to the codebase. We started to tackle tough technical problems and brought aboard [Martin](https://github.com/mamhoff), [Thomas](https://github.com/tvdeyen) and [Alberto](https://github.com/kennyadsl) - three incredibly talented  and experienced individuals to help guide the project.

# Looking forward
These were ambitious plans and still are. The needs of a platform like Solidus are complex and evolve over time, and so should our goals.

As announced at SolidusConf 2017, our growing community has growing needs like better documentation and an improved website. We look forward to sharing our plans for these in detail with you.

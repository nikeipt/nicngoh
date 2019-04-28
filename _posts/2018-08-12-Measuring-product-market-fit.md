---
layout: post
title: Measuring product market fit
tags: [Growth, Product Market Fit]
---

### How do we know we've hit product/market Fit?

Recently read an interesting article by Rahul Vohra: https://firstround.com/review/how-superhuman-built-an-engine-to-find-product-market-fit/ around the topic of product market fit.


Product/market fit is one of those conundrums where you know what it looks like but most of those indicators are post launch. I think one of the golden questions is always how do you know what product market fit looks like before launch or what does that benchmark look like.

It's one of the questions that I've been grappling with and I found this article really provided a great framework around giving you an indicator on whether you've hit it before launch.

The article is quite lengthy but one of the key takeaways was from Sean Ellis.

>  Instead, Ellis had found a leading indicator: just ask users “how would you feel if you could no longer use the product?” and measure the percent who answer “very disappointed.”

What he found after benchmarking a hundred startups is that the magic number is 40%. Companies that were above that threshold tended to have numbers above the 40% benchmark. Slack users were asked and responded at 51% would be very disappointed to never use the product again.

Once they knew this number they sent out an email to their users with some questions:

> 1. How would you feel if you could no longer use Superhuman?
A) Very disappointed
B) Somewhat disappointed
C) Not disappointed

> 2. What type of people do you think would most benefit from Superhuman?

> 3. What is the main benefit you receive from Superhuman?

> 4. How can we improve Superhuman for you?

Which really allowed them to take a look at their customer segments and start moving that needle on the very disappointed users.


#### Segment to find your supporters and paint a picture of your high-expectation customers.

With early stage marketing the data can be a bit murky, especially if the product is free. A lot of people sign up without a real need for your product or the main benefit might not really speak to you.

The goal for the Superhuman team was to find these pockets of users that fell into "Very disappointed" and paint as vivid a portrait of them as possible. The 2nd question in the survey really allows them to nail that because for those users that are very disappointed, the answer to the 2nd question is themselves. Using these responses allowed Superhuman to build a profile of a high expectations customer.

Using this profile they focused on supporting this customer above all else which I thought might be counter intuitive. After all, wouldn't you want to focus on those that didn't get it? They represent a bigger part of the pie and your power users are already in your camp. The words below come from Paul Graham:

>“When a startup launches, there have to be at least some users who really need what they're making — not just people who could see themselves using it one day, but who want it urgently. Usually this initial group of users is small, for the simple reason that if there were something that large numbers of people urgently needed and that could be built with the amount of effort a startup usually puts into a version one, it would probably already exist. Which means you have to compromise on one dimension: you can either build something a large number of people want a small amount, or something a small number of people want a large amount. Choose the latter. Not all ideas of that type are good startup ideas, but nearly all good startup ideas are of that type.”
>“In theory this sort of hill-climbing could get a startup into trouble. They could end up on a local maximum. But in practice that never happens. … The maxima in the space of startup ideas are not spiky and isolated. Most fairly good ideas are adjacent to even better ones.”

I don't know if I necessarily agree, but often times I find myself in the post launch point of a product so it will be interesting when my team releases the mobile app.



#### Analyze feedback to convert on-the-fence users into fanatics.

Superhuman was still below the 40% threshold and so leveraged the profile to understand why this subset really loved their product and hopefully move more people into this segment.

2 core questions that came up were:
> Why do people love the product?

>What holds people back from loving the product?

In conjunction with the 3rd question of their survey which was "What is the main benefit you receive from Superhuman?".

They polled the answers and created a word cloud:
[![Word Cloud](/post images/2018-08-12-Measuring-product-market-fit/word-cloud.png)]

and what they did next was **we decided to politely pass over the feedback from users who would not be disappointed if they could no longer use the product.**

The logic being that the users that don't particularly care about your product shouldn't distract you from your primary benefit. This leaves you with the 'somewhat' disappointed users and echoes some of the lessons from Alex Schulz (VP of growth marketing) where he says focus on your marginal users.

They then got the 'Somewhat users' and once again split them using the key benefit as the divider. For the users that speed was _not_ the main benefit, they were discarded since the main product benefit did not resonate with them. Getting the other 'Somewhat users' they then focused on the 4th question of the survey which was "How can we improve Superhuman for you?". Aggregating the results gave them this word cloud.

[![Feature request Word Cloud](/post images/2018-08-12-Measuring-product-market-fit/Feature-request-word-cloud.png)]

Which really drilled down to the lack of a mobile app. Other things that weren't obvious were stuff like integartions and attachment handling which ended up in the long tail of feature benefits. One of the key things was getting this info and feeding it back to the roadmap.  


#### Build your roadmap by doubling down on what users love and addressing what holds others back

In order to cater the product to those marginal users, Superhuman split their product roadmap. Half would be on what holds users back from loving your product and the other half on what kept them there in the first place. I imagine that this is a hard balance to strike. While it sounds simple I'm also thinking of the other overhead that would arise in the normal course of a sprint like bugs, spec creep or technical debt. Giving half of your roadmap to marginal users is a big call but it certainly sounds promising in this study.



#### Repeat the process and make the product/market fit score the most important metric

From there it was a simple manner of continuously iterating on this feedback loop and taking stock of where the "Very disappointed" users sat at. For Superhuman it become the most visible metric to everyone and it would be polled continuously and within 3 quarters their score went from 22% to almost 58% which is an astonishing jump.  

I found this article really interesting and I'll be revisiting in the next few months. Currently we have a mobile app that's about to launch out to the public however part of the feedback that we're getting is that you wouldn't necessarily download an app that is at parity with the mobile website. After all, what's the point? What native functionality are you taking advantage of?

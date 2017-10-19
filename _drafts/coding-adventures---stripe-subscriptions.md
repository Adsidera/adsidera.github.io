---
layout: post
title: Coding Adventures - Stripe Subscriptions
date: 2017-08-31 00:00:00
author: Adsidera
excerpt: My lazy approaches to Stripe Subscriptions in a production Rails App
---


And then my boss asked me to create the payments interface for her future clients.

I thought of Stripe as third party tool to handle safely payment transactions.

I used it some years before in a demo online shop app, the basic Stripe checkout button.

This time it was different, as our website is offering subscriptions to a service.

I am a lazy developer, my approach is finding the easiest (though better) solutions for the problems I face.

Easiest solutions doesnt mean in any case wrong solutions, solutions that break after a while, lets say the most elegant ones.

If I find myself writing too many lines of code then I ask myself: "is it right?"&nbsp;

If I find myself writing some code that repeats itself then I know it is wrong

I quite easily implemented the Stripe checkout button with a service that I called "stripe_tool.rb"

&acute;&acute;&acute;

&nbsp;

triggered in my controller.

That would just work for one plan, not for all plan.&nbsp;

I did just implement a &acute;subscribers_controller.rb&acute; on my &acute;companies&acute; but the controller did not correspond to any model.

&nbsp;
---
layout: post
title: Coding Adventures - A Simple Form with STI oh yeah!
date: 2017-08-31 00:00:00
author: Adsidera
excerpt: 'My laziness brought me considering single table inheritance, but...'
---


My laziness brought me considering single table inheritance (STI for friends), for the creation of a resource that was basically a copycat of another one. I was working to project involving theatre productions and theatre co-productions. Basically, they shared almost all the same attributes, with the sole difference that theatre productions (productions for friends) were already staged productions, while theatre co-productions (co-productions for friends) were productions to get staged in the future. Another difference was that productions needed to be either on rent or on sale, while co-productions needed to have a budget specified. I thought of implementing a STI between Production and CoProduction models, as a huge list of shared attributes were involved. Do you have an idea how many features does a theatre production imply?

![](/uploads/versions/schermata-2017-12-09-alle-01-14-23---x----696-100x---.png)

This huge number of attributes became a pain when we had to think about how to create a form in our rails app. We decided to go for a wizard form in 5 steps.<br>It worked and works fine for productions. We needed then to use the same wizard form for the CoProduction model.<br>&nbsp;

&nbsp;
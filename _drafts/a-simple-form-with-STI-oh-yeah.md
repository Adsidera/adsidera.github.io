---
layout: post
title: Coding Adventures - A Simple Form with STI oh yeah!
date: 2017-08-31 00:00:00
author: Adsidera
excerpt: My laziness brought me considering single table inheritance, but...
---

My laziness brought me considering single table inheritance (STI for friends), for the creation of a resource that was basically a copycat of another one.
I was working to project involving theatre productions and theatre co-productions. Basically, they shared almost all the same attributes, with the sole difference that theatre productions (productions for friends) were already staged productions, while theatre co-productions (co-productions for friends) were productions to get staged in the future. Another difference was that productions needed to be either on rent or on sale, while co-productions needed to have a budget specified.
I thought of implementing a STI between Production and CoProduction models, as a huge list of shared attributes were involved.
Do you have an idea how many features does a theatre production imply? 

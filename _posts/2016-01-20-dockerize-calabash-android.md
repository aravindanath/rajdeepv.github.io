---
layout: post
title: "Mac, Docker and Calabash"
description: ""
categories: automation docker calabash
excerpt_separator: <!--more-->
---

At Badoo, we use Calabash for automated Android application testing. One of our goal is to make it super easy for developers to run these tests in one command without going through the pain of setting up a test-scripting environment (Installing JDK, Android SDK, Ruby, and praying that nothing else has been added since the documentation was written). The two obvious choices were Vagrant and Docker. Speed of execution was one of the main criteria for us, so we ended up choosing Docker.  

Most of the people in our team use Mac laptops and setting up Docker with Calabash-Android on Mac is not straightforward. 

In [this](https://techblog.badoo.com/blog/2016/12/14/how-to-dockerise-calabash-android-on-mac-os/) article which I wrote on Badoo's tech blog, I have shared the solutions we implemented.
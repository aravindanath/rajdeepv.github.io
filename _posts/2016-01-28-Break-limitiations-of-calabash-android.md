---
layout: post
title: "Breaking Limitations Of Calabash-Android"
description: ""
categories: automation calabash uiautomator
excerpt_separator: <!--more-->
---

Two of the most popular drivers for Android app automation are Appium and Calabash. While both have their pros and cons, their major limitations are:

Calabash: Can only drive UI which is part of the application under test; in particular there is no support for testing notifications.
Appium: Cannot call backdoor methods in the application like Calabash (https://developer.xamarin.com/guides/testcloud/calabash/working-with/backdoors/#backdoor_in_Android). Backdoors are very helpful to set the state of application under test.
 
<!--more-->
We have been using Calabash for automated testing at Badoo since before Appium existed. The stability of Calabash is great and it’s still faster compared to Appium, so we don’t want to migrate. But, to automate a feature-rich application like Badoo, we had to overcome the ‘only application UI’ limitation of Calabash.

I have patched calabash-android server with UIAutomator2 and solved this issue

Please follow my post [here](https://techblog.badoo.com/blog/2017/01/24/break-limitations-with-calabash-android/#disqus_thread) on Badoo tech blog.


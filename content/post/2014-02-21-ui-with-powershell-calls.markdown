---
author: ewmanning
comments: true
date: 2014-02-21 14:28:58+00:00
layout: post
link: https://edwardmanning.wordpress.com/2014/02/21/ui-with-powershell-calls/
slug: ui-with-powershell-calls
title: UI with Powershell Calls
wordpress_id: 153
categories:
- Wiki
tags:
- Code Design
- Powershell
---

(From internal blog - 5 January 2012)

All Microsoft applications are now written so the admin functionality is executed via powershell. The UI simply calls these powershell scripts.

Advantage is that full functionality of the applications can be scripted instead.
Used to be the case that the scripting was bolted on afterwards. This meant that the scripting could not always perform the same tasks as the UI could.

![ui-ps-code](/static/2014/02/ui-ps-code.png)

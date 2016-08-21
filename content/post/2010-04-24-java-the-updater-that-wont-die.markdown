---
author: ewmanning
comments: true
date: 2010-04-24 09:50:47+00:00
layout: post
link: https://edwardmanning.wordpress.com/2010/04/24/java-the-updater-that-wont-die/
slug: java-the-updater-that-wont-die
title: Java - The updater that won't die...
wordpress_id: 59
categories:
- Windows
tags:
- java
- windows vista 32bit
---

<!-- ![Java Control Panel Before](/static/2010/04/javacontrolpanel_24-04-2010_10-35-14.png)  -->

Well, I've been having problems with Java the last couple of weeks.

No, I don't want to install every point release.

When I say "Do not update", I really mean it.

Seems Java's hard of hearing. Despite unchecking the "Check for Updates Automatically" check box, it was still checking for updates and trying to install them.

Turns out that Java's Control Panel will only accept changes made by Administrators, so any changes you make will be quietly ignored.


#### Solution (for Vista 32bit):


Click "Start".

Copy "C:\Program Files\Java\" into the search area at the bottom.

Open the bin folder inside the highest JRE release number (_jre1.6.0_07\bin_ in my case).

Right click "javacpl.exe" and select "Run As Administrator".

Unselect "Check for Updates Automatically" and click OK. You're done. No more Java updates. You can still update manually from the Java Control Panel whenever you want.

![Java Control Panel](/static/2010/04/javacontrolpanel_24-04-2010_10-22-24.png)  


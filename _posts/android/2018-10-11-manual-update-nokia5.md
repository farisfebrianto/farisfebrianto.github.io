---
layout: post
title:  "Manual Update Nokia 5 (TA-1053)"
categories: Android
image: manual-update-nokia5.png
permalink: /manual-update-nokia5/
comments: true
---

Now my mom got new Nokia 5 phone, thank's to my auntie Luluk for buying it. Nokia 5 alaways regularly got monthly updates, the problem is I don't have wifi connection because the update cannot via cellular networks. Many tricks I've done including tethering wifi from another phone, but it seems android smartly recognized it as cellular network.

How to update it without wifi?, I got the solution <!--more--> with manual download and install OTA update

1. Enable developer mode via Setting > System > Developer options. If it doesn't appear tap the build number at about phone.
![enable-dev-mode](/assets/posts/android/2018-10-11-manual-update-nokia5/enable-dev-mode.png){: .align-center}
2. Select take bug report on developer mode, wait it until finished
3. Copy bug report file to phone storage or via whatsapp or upload to google drive
3. Move to computer and extract it
4. Search keyword "https://android.googleapis.com/packages"
![search-ota-url](/assets/posts/android/2018-10-11-manual-update-nokia5/search-ota-url.png){: .align-center}
5. Copy it to downloader

Once finished, now install the update file

1. Plug Nokia 5 to PC and then boot to recovery mode by type command `adb reboot recovery`
2. If screen showing no command just press volume up + power + home button
3. Select apply update from adb
![apply-update-adb](/assets/posts/android/2018-10-11-manual-update-nokia5/apply-update-adb.png){: .align-center}
4. Type `adb sideload filename.zip`
![adb-sideload](/assets/posts/android/2018-10-11-manual-update-nokia5/adb-sideload.png){: .align-center}
5. Wait until finished
![wait](/assets/posts/android/2018-10-11-manual-update-nokia5/wait.png){: .align-center}

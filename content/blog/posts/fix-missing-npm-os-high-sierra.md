---
title: "Fix missing NPM after upgrading to Mac OS High Sierra"
date: "2018-12-24"
language: en
generate-card: false
tags:
  - 'mac os x'
  - 'troubleshooting'
---
I just upgraded my Mac to OS X High Sierra (10.13.6). Everything seems to work normally, my existing projects run fine (various React apps and a Laravel app on Docker), until I tried to run npm / npx. 

Any npm command returns the error `command not found: npm`. 😱

I checked and found that Node still exists on my machine. I installed Node JS with [Homebrew](http://osxdaily.com/2018/03/07/how-install-homebrew-mac-os/), so I ran `brew upgrade npm`. After upgrading, I ran `npm -v` and confirmed NPM is working again on my machine! 🎉

_Note: If you did not install Node through Homebrew (ie. with installation package from [Node website](https://nodejs.org/en/download)), I recommend uninstalling and doing a fresh install._
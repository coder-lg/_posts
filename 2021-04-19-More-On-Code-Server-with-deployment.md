---
title: More on Code Server with deployment
layout: post
date: '2021-04-19 17:45:00 +0530'
bootstrap: true
author: coder-lg
excerpt_separator: "<!--more-->"
categories:
- vscode-on-cloud
- deployment
- codeserver
- cdr
---

Get to know how to deploy the Code-Server repo on Railway(GitHub account needed!)
<!--more-->

* TOC
{:toc} 
# Beginning

So, a lot of you know about Code-Server, and it is cool but a problem is that you MUST have a Linux distro to use it.
This guide is made for the people who wanna use it without a linux distro like Debian.
## Deployment
Railway is advised and a GitHub account, more advised.
So, go to code-server in GitHub and hit F3. Then search 'deploy' and hit the link. It will take you to another repository by cdr. Then scroll down and hit Railway's see docs. Then hit the Railway icon which is a bullet train. You will go to Railway and login with GitHub. Then scroll down and set private, put a password, and copy this: `https://github.com/cdr/docs.git`

Then hit Deploy and wait. Then, see your bottom right corner for a green popup. When it comes, hit that and you will go to a new site. It will ask for the password you set during deployment, so enter that. You now got Code-Server deployed and running, sir!

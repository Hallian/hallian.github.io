---
layout: post
title:  "AWS CodeDeploy: Practical example"
date:   2017-09-08
excerpt: "One prevalent feature of a DevOps project is deploying your code in an automated fashion. Everybody can setup a CI these days but how do you actually get the code to the server?"
image: "/images/2017-09-08-codedeploy-example/stack.png"
---

One prevalent feature of a DevOps project is deploying your code in an automated fashion. Everybody can setup a CI these days but how do you actually get the code to the server? Too many times have I seen a cron timed bash script that pulls in the new code directly from version control. Or worse yet, it's a process where someone logs in to the server via ssh and does it manually. This is not the way to do it. You really should invest in an actual code delivery tool if you're planning on actively developing the software.

The best code delivery tool I've ran into to date is AWS CodeDeploy. You build a package of your software along with scripts to install it. An agent runs on your server that notices new deployments registered with the CodeDeploy system and takes action to install new versions. Best of all CodeDeploy integrates seamlessly with other AWS systems like Auto Scaling.

Due to the relative difficulty of explaining the process to people with no prior AWS experience, I decided to create an example repository that contains all the required templates and configurations for setting up EC2 virtual servers with application delivery handled by CodeDeploy.

See my [codedeploy-example <i class="icon fa-github"></i>](https://github.com/Hallian/codedeploy-example) repository on GitHub for more.
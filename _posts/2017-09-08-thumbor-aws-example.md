---
layout: post
title: Thumbor AWS Example
date: 2017-09-08
excerpt: After working with a custom PHP resizer script revision 1573, I started looking for a ready made solution that could just be setup with minimal effort. Turns out there is an existing, maintained solution for this task.
image: "/images/2017-09-10-s3-serverless-example/s3-serverless-example.png"
image: "/images/2017-09-08-thumbor-aws-example/stack.png"
---

Every web project that I've been a part of has had the need for resizing images used by the website/webapp. Rather than use an existing solution, everyone seems to think that resizing images is easy and they can implement it in an afternoon with PHP and imagemagick. This naturally results in extended development times and an image resizer that is buggy and vulnerable to exploits.

After working with a custom PHP resizer script revision 1573, I started looking for a ready made solution that could just be setup with minimal effort. Turns out there is an existing, maintained solution for this task. An on-the-fly image manipulating open source software called Thumbor. All you need to do is host it somewhere.

Now, after setting this up for a couple of times on AWS, I started getting tired of re-creating the CloudFormation setup files everytime, so I created an example repository that contains all the necessary files and configurations to quickly get it up and running. This also served as a good material for training sessions that we (PHZ Full Stack) arrange during our monthly sauna events.

See my [thumbor-aws-example <i class="icon fa-github"></i>](https://github.com/Hallian/thumbor-aws-example) repository on GitHub for more.

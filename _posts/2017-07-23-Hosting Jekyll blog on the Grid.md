---
layout: post
title: "Hosting Jekyll on the Grid"
date: 2017-07-23 23:08:11 -0600
categories: en
comments: true
tags: infrastructure
---
Since I started to create this website I have tried several technologies, in a long way, I think is a solution is the most affordable and reliable.

<!-- more -->
My requirements for the website was:
1. No, be tied to a specific platform, for example, WordPress or Drupal. 
2. Be the owner of my data. The preferred way is to store everything in a Git repository. 
3. Simple blogging mechanism, easy as writing a markdown file.
4. Not significant cost.  

Some of the approaches that I have done was doing everything from scratch, the solution was very customizable, however, was very hard to maintain and develop so I moved to [Ghost][1] a blogging platform that supports markdown files and have a nice and simple blogging CMS(Content Management System), It run NodeJS server, I decide to put behind a [Nginx][2] server in a VPS(Virtual Private Server) to enable caching and add a security layer SSL (Security Socket Layer), but as you can think that is not the correct tool for the problem, because we are only hosting and static website with few changes during the time. 

After that I decide to explore [Jekyll][3], mainly for its native support of markdown files and static website generation. So I set up, modified the CSS and HTML files, and as many of you know I'm NOT an avid web developer, but I could do the changes with easiness. 

I still at that time host the site behind the Nginx, but the cheaper VPS out there cost around $5 USD/month, this still has some drawbacks:

1. Expensive for hosting a few HTMLs.
2. Take care of the maintenance of the server.
3. Share space with others VPS.
4. Hard to move from 1 provider to another.
5. Not scalable.

When I started to use the VPS, I chose as an alternative to hosting in some of those hundreds of websites, cheap hosting but not good quality of the service at the other end, AWS, Azure, and GCP were out of the budget, a VPS there is expensive that and VPS in some websites. But I really don't need computing power, because I'm not hosting a DB or providing any kind of service, only a few HTML, JS and CSS files.

I find out that the bucket or blob could be used as hosting and you can set up a custom domain. Definitely, that beat the hosting in the VPS. 

1. Scalable, not matter if the site has 1 user or hundreds.
2. Availability, I set up global replication of the bucket.
3. Security, it provides an SSL certificate and ACL's.
4. Reliable, Pay as you go. I'm paying as low as $0.99/month.

![aws architecture][AWS]

## Guides
* [AWS][4]
* [GCP][5]

[1]:https://ghost.org/
[2]:https://nginx.org/en/
[3]:https://jekyllrb.com/
[4]:http://docs.aws.amazon.com/AmazonS3/latest/dev/WebsiteHosting.html
[5]:https://cloud.google.com/storage/docs/hosting-static-website
[AWS]: /img/aws-architecture.PNG "AWS static hosting"
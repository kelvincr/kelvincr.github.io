---
layout: post
title: "Illusion of online Privacy"
date: 2017-08-08 21:40:11 -0600
categories: en
comments: true
tags: privacy
---
Be connected is part of most people now-days. Doing things online is easier than ever. Things like banking, buying stuff, communicate with others are a few clicks away. All that came with a hidden cost for many people do not know: *lost of privacy*. I would like to share some thoughts and ideas on that.    

<!-- more -->
![Illusion of Privacy][Privacy]

I consider security and privacy are a big concern nowadays, governments eavesdropping communications, cyber-crime increasing every day, Big corporations 'being Evil' tracking every click user does to try to monetize it. Not much people are taking care of that. I was like that until I start getting interesting in security. Maybe many of you can think, I am a silly person worrying about that or I am hiding something, nor of them. I would like to explain that,

Imagine you are at home dining with your family talking how was everyone day or planning a weekend trip, and suddenly a stranger gets into your house because you forgot to close your door. Do you think that's normal in our society? It's  the same situation with your *connected life*, some government, company or individual believes that has the attribution to make that interfere with your life.

## Tracking on searches.
Almost all big brand browsers like Google, Bing, and Yahoo, track all your search habits, at the begging that was used to make more accurate responses, however it has become a way of doing money, you are a tagged dot in their constellation of users, whenever someone want to promote certain information, i.e. a product for a specific group of people the range of age from x to y from this places. They will offer that services, I am not against that, because they are a business and they need to have a proper model to maintain their self, but is not the only model, that's why I would like to share some alternatives, 

1. [DuckDuckGo][1] doesn’t use cookies to identify you, and it discards user agents and IP addresses from its server logs
2. [Startpage][2] searches Google for you – when you submit a search, StartPage submits the search to Google and returns the results to you.

In both cases, authorities are able to know who are doing the searches by requesting to providers to intercept traffic and determinates your identity.

##  Email privacy.

In that specific topic, there are 2 concerns, the first one is the vulnerability of your email hosted with a provider in a country with flexible laws to allow a government to seek everywhere, I have to said they should develop more efficient ways to search and find people related with illegal activities. Exhausting searching is not the best and the result could not be the expected. The content of email is accessible for the provider at anytime, before continue I would like to introduce a concept, *zero-knowledge architecture*, this is when the provider does not know anything about the information stored in their service, It means only the owner is able to read that information, if that is read by someone else is going to be unreadable, because the information is encrypted with the secure key of the owner. 

One email service provider that aimed to control that is [ProtonMail][3], you will use 2 keys to access the service the first one is for authentication process, the second one in for decrypted your mailbox it is done in your browser using JavaScript technology. Beside of that the servers are hosted in Switzerland very restrictive laws in favor of privacy, the free service comes with 500MB. 

The second concern is a known issue of the email protocol, the metadata of the email is exposed, even if the content is encrypted end-to-end. 

## Storing your information.

During our life, we store information, some things are personal documents, email, family pictures, or part of professional stuff this need to be secure and accessible anywhere and anytime with low risk of losing that family memories or that important project for a customer, besides of that we need security when we store the information. Out there are many SaaS platforms that offer even free storage, like Dropbox or google drive for mention some. However all that information is not secure of unauthorized access again *zero-knowledge* could help but we need to take into account an important consideration, if we lost the master key we lost everything and there no way to recover the information.  

[1]:https://duckduckgo.com/
[2]:https://startpage.com/
[3]:https://protonmail.com/
[Privacy]:/img/privacy.jpg "Privacy"

---
layout: post
title:  "Recreating the Infamous Facemash"
date:   2014-7-27 01:02:35
categories: creative
---

Yesterday was a hell of a day. We re-created the infamous Facemash in less than 4 hours. The idea to re-create Facemash started with a debate  among my roommates who are from different states of India.  I started shouting to Bhagyraj and Harish that Kerala is the most beautiful state in India. Well, even though its is true :p my roommates did’t agree with that.  We thought of a solution to settle this problem but none seemed working. At last I came up with the most stupid solution one can ever find. Recreate Facemash for rating pictures of our states.  Bhagyraj and Harish shouted “Hell, Yeah”  and we started working on the site.

<img src = "/images/comparo.png">

 

We used the famous Elo algorithm for rating the pictures.  If you are not familiar with the Elo algoritham, then Google it.  I will try to explain the basic implementation of Elo algorithm for rating players. If you want to rate two players then the new rating of player A looks something like this.

<img src = "/images/elo-rating.png">

K is the “k factor”, an arbitrary multiplier (a higher k factor means higher rating volatility), S is the total score in a rated event, and E is the total expected score in a rated event, which is calculated by

<img src = "/images/elo-rating-vishnu.png">

We implemented the website in PHP and Twitter Bootstrap.  Once the website was done we got suggestions from some alpha testers to include the pics of College girls instead of pictures of different states from where we hail.  Well, as we had complete respect for the girls in our campus and didn’t want to hurt anyone we decided to go for rating film stars at the last minute before the launch  instead of pictures of states.

Finally we launched the website at around 1 AM and got a thousands hits a few minutes later.
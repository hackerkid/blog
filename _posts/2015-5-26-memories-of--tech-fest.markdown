---
layout: post
title:  "Beautiful Memories of the first Tech Fest"
date:   2015-3-26 02:15:35
categories: events
---

The first Tech Fest of IIIT Allahabad Aparoksha turned out to be quite awesome. My experience started with Coldfire which was the first offline Technical event of Aparoksha.  Coldfire was an event in which you have to identify the vulnerabilities in web applications. Even though I have a little bit experience in developing small web applications We had very little knowledge in penetration tests. But the unexpected happened on that day. I and my roommate Bhagyaraj emerged as the winner of Coldfire cracking all the 10 problems in Coldfire. The first two questions was based on injecting javascript code through the GET variables.

{% highlight javascript %}
<scr</script>ipt>alert('Hacked :p')</scr</script>ipt>
{% endhighlight %}

Some questions involved encrypting the javascript code to ASCII and decrypting again and evaluating with the help of `eval` function. There were also a few questions on SQL injection which turned out to be quite simple. In one question all we needed was to change the input the username as * which retrieved all the rows.

There were some tricky questions which involved finding the MAC address and hostname of the server. We were meant to find the MAC address by injecting to server a call to `phpinfo()`. But since the server was in the same computer lab as we were in we just used the ' arp -an ` command to find the mac address of the computers in the network. Since the IP address was already known the rest of the part was pretty simple. One question was to find the Apache version of the server. We couldn't find a way to retrieve this information so we simply brute forced the possible Apache versions.

<img src = "/images/codeshow.jpg">

The other event which I took part was IT Quiz. Unfortunately our team suffered an early second round exit. Then came the Codeshow finals. Codeshow was an ACM ICPC styled competition. There was a prelims which took place a few weeks before. Around 20 teams which were able to solve more than 3 problems were chosen for the onsite. We were not able to get a prize but it was really an awesome experience.

I and Bhagyaraj also teamed up for Confedarore, a debugging competition based on Android. As I was not comfortable with Android Bhagyaraj began to analyze the code while I began to document the bugs. Finally we were able to fix around nine bugs. We created the patch files and send it to the organizers almost on time. After some time we got call from organizers that we were placed second in the contest. That was our second win the tech fest.

Hackathon which was one of the event I was looking to participate got canceled in the last moment. We were not able to attend the back end development competition 'Backbone' due to the conflict in timing with Codeshow. Looking backward, the Techfest teached us  a lot of things in a very short period of time. It was really three days of awesomeness.




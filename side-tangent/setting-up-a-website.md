## Hosting a web site
This Document will talk about the amazing time I had learning how to host my own website on my home server.

### The goal
The main objective was to host a website on my server using Apache and then use Cloudflare tunneling to route it to my domain name: "kae-sec.com".

### The good
Starting off, everything was going pretty well, httpd was running and there were a few permission errors but they were quickly resolved. However...

### The bad
Basically everything that could have gone wrong from here, did go wrong. After installing the cloudflared service, the first thing I noticed was that a cloudflare user and service had not been created on install - luckily this is a pretty easy fix. 

---
layout: post
title: "Dispatches On Scalability - August 7th 2014"
description: "Scalability news and updates from August 7th 2014"
headline: "From the fluentd to penetration testing NoSQL stores."
category: dispatches
tags: 
  - dispatches
  - mongodb
  - ssl
  - https
  - aws
  - messages
  - cloudflare
  - security
imagefeature: vintage-computers.jpg
imagecredit: mariemosley
imagecreditlink: "https://www.flickr.com/photos/mariemosley"
comments: false
mathjax: null
featured: false
published: true
---

Google has [announced that it is to begin to factor HTTPS / SSL into its rankings](http://googleonlinesecurity.blogspot.co.uk/2014/08/https-as-ranking-signal_6.html) causing an obvious mad dash by every SEO optimiser to ensure the sites they represent are servicing secure requests. [CloudFlare, the DDoS / DNS / CDN provider,](http://blog.cloudflare.com/google-now-factoring-https-support-into-ranking-cloudflare-on-track-to-make-it-free-and-easy) have responded with an announcement that they intend to provide free SSL certificates and protocol enablement to everyone using their service. This should instantly enable millions of sites to the make use of the enhanced security which is excellent news for all kinds of reasons and the [performance and scalability impact should be near to zero.](https://www.imperialviolet.org/2010/06/25/overclocking-ssl.html)

[There an article on the AWS Blog](https://aws.amazon.com/blogs/aws/all-your-data-fluentd/) about Fluentd and how it can be used to stream a vast amount of log data from decoupled components. Fluentd is an open source data collector designed to unify log management and has a pluggable architecture to allow that data to be stored in a vast array of different datastores. Obviously they pitched its use within there IaaS, however, it is a component entirely ready to be deployed anywhere and can ingest a massive number of messages (~15,000 events/sec on a single core.) [There is an excellent into on the Fluentd website](http://www.fluentd.org/architecture) and a good explanation around how it can [reduce complexity in log management](http://www.fluentd.org/blog/unified-logging-layer) for  typical multi-component architectures.

Planet Cassandra released a [nice little talk about the use of messaging within SimpleReach](http://youtu.be/jFrC1rHZEcM) in order to cater to their 3.75 billion page views a month and 7 billion events per day. In the video Eric Lubow, CTO of SimpleReach, discusses why messaging is an important part of a distributed system stack explaining that, they are often overlooked because the prevailing sentiment is that the storage and processing engines are the most important aspects of the system. He looks at the impact on scalability, elasticity, deliverability and redundancy. 30 minutes well spent!

Finally, for those of us with a bit of a security bent, Francis Alexander gave an interesting presentation around [penetration testing and exploiting NoSQL datastores](http://youtu.be/WWAdMqr_vAg) at the Hack in Paris conference. He gives good coverage of Good coverage of MongoDB, CouchDB and Redis and highlights quite a few security complications. Interesting watching for anyone who relies on the current grate and good of the NoSQL world.
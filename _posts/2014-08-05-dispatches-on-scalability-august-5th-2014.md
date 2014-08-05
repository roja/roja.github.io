---
layout: post
title: "Dispatches On Scalability - August 5th 2014"
description: "Scalability news and updates from August 5th 2014"
headline: "From the thoughtworks technology radar to ."
category: dispatches
tags: 
  - dispatches
  - mongodb
  - tokumx
  - technology radar
  - consensus
  - microservices
  - riak
imagefeature: nova-1200-lookalike.jpg
imagecredit: timonoko
imagecreditlink: "https://www.flickr.com/photos/timonoko"
comments: false
mathjax: null
featured: false
published: true
---

Today marks the release of the [ThoughtWorks Technology Radar](http://www.thoughtworks.com/radar/#/ "ThoughtWorks Technology Radar"), there annual review of the technology world, what they are adopting and what they are dropping. Bringing together there collaborative knowledge in building architectures and consulting for clients it's a hugely useful resource and a must read for anyone in tech. If nothing else it if a cracking vehicle for discovering new techniques and technologies to deep dive into.

[MongoDB, has hired a new chief executive, Dev Ittycheria](http://venturebeat.com/2014/08/05/mongodb-dev-ittycheria/ "MongoDB, has hired a new chief executive, Dev Ittycheria"), who replaces [Max Schireson who has left for personal reasons](http://maxschireson.com/2014/08/05/1137/ "Max Schireson who has left for personal reasons") as he explains in an interesting article about striking the right balance between work and life. A lesson many of us could learn. There is also an interesting article on their site about [making use of MongoDB's geo capabilities to perform music recommendations](http://blog.mongodb.org/post/93874668363/mongodb-the-soundwave-music-map "making use of MongoDB's geo capabilities to perform music recommendations"). Well worth a read.

There is a fantastic series of posts on the tokutek blog about the new [consensus algorithm they have developed for TokuMX and MongoDB](http://www.tokutek.com/2014/07/introducing-ark-a-consensus-algorithm-for-tokumx-and-mongodb/ "consensus algorithm they have developed for TokuMX and MongoDB"), similar to Paxos and heavily influenced by Raft, built to handle replica set elections and failovers in TokuMX. There are 3 additional posts going into [the basics](http://www.tokutek.com/2014/07/explaining-ark-part-1-the-basics/), [why they did it](http://www.tokutek.com/2014/07/explaining-ark-part-1-the-basics/), and [when it can fail](http://www.tokutek.com/2014/07/explaining-ark-part-3-why-data-may-be-lost-on-a-failover/).

InfoQ have released an [eMag on Microservices](http://www.infoq.com/minibooks/emag-microservices) designed to show us that they are more than just a passing fad. Not just an extension of Service Oriented Architecture and more than just smaller surface areas for service deployments. Lofty claims! That said, it's free and offers a good general overview of some of the pro's and con's.

Last but no means least, Basho, everyone’s favourite erlang shop, have released a [new version of their Riak cloud storage layer](http://docs.basho.com/riakcs/latest/). If you are stuck in an enterprise world with no ability to use S3, it may just be a lifesaver!

That’s quite enough for today!
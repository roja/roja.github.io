---
layout: post
title: "Dispatches On Scalability - August 11th 2014"
description: "Scalability news from August 11th 2014 - Presentations from QCon New York, CoreOS, Azure with Node.js and Will HBase win the NoSQL race?."
headline: "Presentations from QCon New York, CoreOS, Azure with Node.js and Will HBase win the NoSQL race?"
category: dispatches
tags: 
  - dispatches
  - vert x
  - riak
  - apollo
  - coreos
  - docker
  - azure
  - hbase
  - netflix
imagefeature: blue-to-uv-laser-stage.jpg
imagecredit: fatllama
imagecreditlink: "https://www.flickr.com/photos/fatllama/"
comments: false
mathjax: null
featured: false
published: true
---

InfoQ has had a fantastic few days and has pushed out a whole host of excellent content from there QCon 2014 in New York. First there is a presentation by Tim Fox from Red Hat around using the lovely reactive java / polyglot, node.js inspired, framework [Vert.X to develop high performance reactive web applications.](http://www.infoq.com/presentations/performance-reactive-vertx?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global) Next up [Aviran Mordo introduces Wix's architecture,](http://www.infoq.com/presentations/wix-architecture?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global) a highly available eventually consistent system, along with patterns for rendering many websites with a relatively small number of servers, handling 700M HTTP requests/day and have some tight SLA's for their huge user base. [Sean Cribbs discusses the theory behind several new data types introduced within Basho's version 2.0 of Riak.](http://www.infoq.com/presentations/data-modeling-riak?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global) Aiming to reduce the "difficulty" when it comes to operating data storage and conflict resolution when running large scale deployments. Finally [Jeff Johnson introduces Apollo, facebooks hierarchical NoSQL data system](http://www.infoq.com/presentations/scale-facebook-big-data?utm_campaign=infoq_content&utm_source=infoq&utm_medium=feed&utm_term=global) meant to deal with their vast distributed storage needs. Built using Thrift2 and making use of a Paxos-style / Raft quorum protocol for consistency and RocksDB for K/V storage it looks like they are using if for all sorts of internal systems.

[CoreOS have released the first stable build of their entire re-architected, Linux distribution](https://coreos.com/blog/stable-release/), providing docker container management, service discovery with Etcd the highly-available key value store, and process management with Fleet, a distributed init system for clusters. [There is lots more detail about CoreOS and what they aim to achieve in the long run,](https://coreos.com/) it is however fantastic to see them progressing towards their first full release as there end goal is not too different than clustered deployment utopia.

Bruno Terkaly has written a nice little getting started article for [making use of azure service bus from a node.js application deployed into azure web sites.](http://blogs.msdn.com/b/brunoterkaly/archive/2014/08/10/node-js-in-azure-web-sites-and-service-bus-installing-tools-and-reading-messages-from-cloud-hosted-queues.aspx) He looks though the basics including how to setup queues and even how to setup web matrix for easy development.

[Will HBase win the NoSQL race? Is there a race? Andrew J. Brust thinks there is](http://gigaom.com/2014/08/10/is-hbases-slow-and-steady-approach-winning-the-nosql-race/) and sets about answering his own question focusing on the momentum in the HBase world right now with innovative add-ons / layers which exploit the HBase engine; Hive, MapR, Reactor etc... I can't say I am entirely convinced however it's a nice list of links to some fantastic solutions. Especially worth checking out is [Continuuity Reactor](http://www.continuuity.com/products/reactor) and there [newly released](http://www.slideshare.net/alexbaranau/transactions-over-hbase) open source [HBase transaction engine Tephra.](https://github.com/continuuity/tephra)

Finally [a nice little video presentation about the use of micro services at NetFlix.](https://www.youtube.com/watch?v=LEcdWVfbHvc)

Fin.



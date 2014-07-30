---
layout: post
title: "Dispatches From The Edge - July 16th to July 30th 2014"
description: "Some of interesting things appearing in tech scene during the fortnight ending July 30th 2014"
headline: "From elastic search to building your own cdn all engineered for growth."
category: dispatches
permalink: /dispatches-from-the-edge-july-16th-to-july-30th-2014.html
tags: 
  - dispatches
  - elasticsearch
  - couchdb
  - hyperdex
  - aerospike
  - spark
  - cdn
  - graph databases
  - collaborative-filtering
imagefeature: nova-1200-lookalike.jpg
imagecredit: timonoko
imagecreditlink: "https://www.flickr.com/photos/timonoko"
comments: false
mathjax: null
featured: false
published: true
---

## Scalability in software ##

The ever dependable [elasticsearch released version 1.3.0](http://www.elasticsearch.org/blog/elasticsearch-1-3-0-released "elasticsearch released version 1.3.0")  bringing a whole host of performance and security improvements to one of the most useful tools we have for bringing search to large web deployments. There aggregations are really coming of age and offering a simple, explorable and high performance alternative to traditional approaches especially when coupled with their kibana dashboard. Watch out splunk!

In a somewhat unexpected move [cloudant released "cloudant script"](https://cloudant.com/blog/couchdb-and-mongodb-let-our-query-apis-combine "cloudant released cloudant script") with an intention of bringing mongodb-like queries to their distributed couchdb product. Their aim is to help move towards a unified syntax for NoSQL stores, a lofty goal and a questionable choice in mongo as a paragon of syntax, if it achieves its aim of bringing accessibility to the fantastic couchdb then for the moment at least it looks like a positive pragmatic move.

This fortnight also saw the [alpha release of cockroach.](https://github.com/cockroachdb/cockroach "alpha release of cockroach.") A distributed key/value data store supporting ACID semantics versioning with globally distributed consistency and survivability as a core design goal. It's named for obvious reasons given its aim and directly targets automated resilience with mega simple administration and configuration. It's built by ex-googlers who worked on spanner and colossus so it’s defiantly going on the watch list.

[Hyperdex, the clustered, transactional, document and data structure store](http://hyperdex.org/NEWS/ "Hyperdex, the clustered, transactional, document and data structure store") hit it's 1.4 release bringing performance improvements to the novel peer-reviewed indexing technology. Even if you have no intention of using the store it's absolutely worth taking a look at the paper which formalises there approach, it is very accessible but shows an entirely new way of creating indexes which are by their definition distributed.

Last but by no means least, [Aerospike decided to adopt a different business model](http://www.aerospike.com/blog/entrepreneurs-break-all-the-rules-aerospike-goes-open-source "Aerospike decided to adopt a different business model") and made its high performance scalable data store open-source. Their performance claims are extraordinary but they claim to have benchmarks to back them and the community seems to agree, at least in orders of magnitude!

## Thoughts on scale ##

Recommendation engines, relevant products, it seems everyone is interested in collaborative filtering at the moment. The chaps at [databricks have written a little starter artical](http://databricks.com/blog/2014/07/23/scalable-collaborative-filtering-with-spark-mllib.html "collaborative filtering in mlib") on how it can all be achieved through the use of Spark Mlib, it cuts right to the facts and shows off some of the power behind the spark cluster computing system and the machine learning tools available in mlib.

Big Data. No, not a billion rows in a database, try 20 terabytes of new data and 10 petabytes of data overall. This [excellent read from the people at pinterest](http://engineering.pinterest.com/post/92742371919/powering-big-data-at-pinterest "big data at pinterest") outlines how they leverage Hadoop and AWS to handle their vast data acquisition and storage challenges and power some of their most important user facing features. If nothing else it's fantastic to see how their original platform handled there huge rate of growth!

The CDN has become the mainstay of delivering web content for most of the major players on the web. By offloading the delivery of simple static assets it’s possible to free up systems best used to build dynamic pages and with more advanced techniques it's even possible to improve the performance of the dynamic content too. In [this article Chris Ueland](http://www.scalescale.com/rolling-your-own-cdn-build-a-3-continent-cdn-for-25-in-1-hour "build your own cdn"), president of maxcdn, walks though how to build up the basics of a CDN using just $25 of hosting and an hour of your life. It's simple, far from production ready, but gives a good insight into the fundamentals of how what a CDN really is underneath all the marketing.

Graph databases seem to be making a comeback and not without reason. In this blogpost we [explore if there is a different approach to exploring events](http://snowplowanalytics.com/blog/2014/07/28/explorations-in-analyzing-web-event-data-in-graph-databases "web events in a graph database") by storing them as a graph and leveraging the powerful traversal powers of Neo4J to build new insight from the same old data.

Well that about wraps up another fortnight. Hope you found some of the links interesting!
+++
author = "David Makogon"
categories = ["Nosql", "Data", "Talks", "Build", "Recordings"]
date = 0001-01-01T00:00:00Z
description = ""
draft = false
image = "/images/2016/04/relationalcar.png"
slug = "build-session-json-document-modeling"
tags = ["Nosql", "Data", "Talks", "Build", "Recordings"]
title = "//build/ session: JSON Document modeling"

+++


[Ryan CrawCour](https://twitter.com/ryancrawcour) and I recorded a fun session for //build/ 2016:

[Modeling Data for NoSQL Document Databases](https://channel9.msdn.com/Events/Build/2016/P468)

Document databases are non-relational databases that store data as collections of JSON documents, such as:

```
{
   "id": "P468",
   "title": "Modeling Data for NoSQL Document Databases",
   "speakers": [
      {"name": "David Makogon"},
      {"name": "Ryan CrawCour"}
   ],
   "synopsis": "...",
   "tags": ["data"],
   "level": 200
}
```

If you hail from the relational database world, this type of embedded, denormalized document might seem a bit jarring!

Turns out: There's quite a bit to consider when modeling documents, especially when the intent is to store and query them in a database. For example:

- Embedding vs referencing (yep, you can still reference data in other documents)
- Normalization vs denormalization
- Homogeneous vs heterogeneous data

In this short (30 minute) talk, Ryan and I dive into these specific challenges. We also walk through some real-world use cases we've helped our partners solve, such as:

 - Hierarchical data
 - Keyword / tag searching
 - Telemetry
 - Logging


+++
author = "David Makogon"
categories = ["Azure", "Conference", "Mongodb", "Nosql", "Azure Tables", "Neo4j", "Nosqlnow", "Polyglot Persistence", "Storage"]
date = 0001-01-01T00:00:00Z
description = ""
draft = false
slug = "no_sql_now_talk_summary_and_links_polyglot_persistence_in_windows_azure"
tags = ["Azure", "Conference", "Mongodb", "Nosql", "Azure Tables", "Neo4j", "Nosqlnow", "Polyglot Persistence", "Storage"]
title = "NoSQL Now! talk summary and links: Polyglot Persistence in Windows Azure"

+++


Thanks to those who attended my session on Polyglot Persistence in Windows Azure today at the **[NoSQL Now!](http://nosql2013.dataversity.net/)**conference in San Jose. Here are slides and a few notes from today's session and follow-on questions. 

<iframe frameborder="0" height="327" scrolling="no" src="https://skydrive.live.com/embed?cid=9153BB9D3667F0EB&resid=9153BB9D3667F0EB%21200960&authkey=AKCw8rinpmrG9FA&em=2" width="402"></iframe> (download ) 
**How will Windows Azure provide NoSQL database support?** 
Today, Azure offers Table Storage as a NoSQL key/value store. Additionally, several partners have begun offering database "as a service" running in Windows Azure. For example, MongoLab and MongoHQ provide Azure-hosted MongoDB, while Cloudant provides Azure-hosted CouchDB. 

Some of these databases are available directly through our partners' web portals, while others have also integrated into the Azure Store as part of the Windows Azure portal. Here's an example of MongoLab's MongoDB integrated in the store: 
[![](http://4.bp.blogspot.com/-Cv2XMg9rgIw/UhZDdkpjfuI/AAAAAAAAA4k/9Joc-YdHfX8/s320/azurestore.png)](http://4.bp.blogspot.com/-Cv2XMg9rgIw/UhZDdkpjfuI/AAAAAAAAA4k/9Joc-YdHfX8/s1600/azurestore.png)For self-hosting, several partners have built virtual machine images, installable via Azure's VM Depot. Here's Neo Technology's Neo4j 1.8: 
[![](http://1.bp.blogspot.com/-um0nzxY49qc/UhZDwVPV9KI/AAAAAAAAA4s/lj7B50VAYQc/s320/vmdepot.png)](http://1.bp.blogspot.com/-um0nzxY49qc/UhZDwVPV9KI/AAAAAAAAA4s/lj7B50VAYQc/s1600/vmdepot.png)**What, exactly, is VM Depot?** 
VM Depot is a repository of community-created Linux-based virtual machine images. In terms of NoSQL, there are a few NoSQL database images available today. For example, you'll find Neo4j, MongoDB, Redis, and Riak. 

**What does VM Depot cost?** 
VM Depot is free: Free to publish images and free to download images to your Azure account. 

**What are the architectural considerations for integrating multiple NoSQL databases in my app**? **Are there standard practices?** 
As the Cloud Ninja Polyglot Persistence project demonstrates, you can choose to either make direct database calls or implement an abstraction layer, implementing such patterns as _repository._ When going with a _repository_ pattern, this allows you to swap out database engines with reduced impact to your existing code base, although it's possible you'll need to make adjustments to your app's data access API. 

**How do I choose a specific NoSQL database implementation? Can you please recommend one?** 
For key/value storage, Azure Table Storage offers massive scale (200TB per namespace) and provides very fast storage and lookup. As for 3rd-party vendor offerings, I really cannot give specific recommendations, but I _can_ offer some food for thought when making your decision: 

* Look at the company's longevity, financials, funding, etc.
* Does the vendor provide Professional Services support?
* How big / popular is the _community?_ Consider forums, web presence, conferences, etc.
* How robust is language support? does the product offer direct API's when using a non-supported language?
* How active is the project? Are there frequent updates? Can you view the code (e.g. OSS)?
* Will the database engine run on your target OS? Some databases may be Windows-only or Linux-only.

**What was that super-cool zooming app you used during your demo???** 
I was using , written by Mark Russinovich. 

**Where can I find more information about the stuff you talked about today?** 
Here are some informational links from today's talk: 

* [www.windowsazure.com](http://www.windowsazure.com/)
* [http://bit.ly/azuretrainingkit](http://bit.ly/azuretrainingkit)
* [http://cn2p.codeplex.com](http://cn2p.codeplex.com/)
* [http://cn2p-web.cloudapp.net](http://cn2p-web.cloudapp.net/)
* [http://github.com/windowsazure](http://github.com/windowsazure)
* [https://dataguidance.codeplex.com/](https://dataguidance.codeplex.com/)
* [http://www.windowsazure.com/en-us/documentation/services/storage/](http://www.windowsazure.com/en-us/documentation/services/storage/)
* [http://bit.ly/neo4jonazure](http://bit.ly/neo4jonazure)
* [http://bit.ly/mongodbonazure](http://bit.ly/mongodbonazure)

There are a few more resources we didn't talk about, but should still be valuable:[Zoomit](http://technet.microsoft.com/en-us/sysinternals/bb897434.aspx)


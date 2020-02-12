+++
author = "David Makogon"
categories = ["Azure", "Mongodb", "Azure Store", "Mongolab"]
date = 0001-01-01T00:00:00Z
description = ""
draft = false
slug = "mongo_lab_extends_windows_azure_mongo_db_offering_with_8_gb_replica_sets"
tags = ["Azure", "Mongodb", "Azure Store", "Mongolab"]
title = "MongoLab extends Windows Azure MongoDB offering with 8GB Replica Sets"

+++


If you're using MongoDB in Windows Azure, you may already be aware that, aside from self-hosting, you can take advantage of Hosted MongoDB. One such provider, MongoLab, has been offering a _free-tier_ offering, with up to 500MB, for a while now. However, that might be a bit limiting if your app is past the "just getting started" point. 

Good news: MongoLab now has a Replica Set offering for Windows Azure, supporting databases  up to 8GB! You can set this up through the Azure Store as well as through the MongoLab portal. If you go the Store route, you'll see both the Free and Paid options: 

[![](http://3.bp.blogspot.com/-MulBuBYT42s/UdxMJYAZynI/AAAAAAAAA38/ATfvnGvnRHg/s320/mongolab1.jpg)](http://3.bp.blogspot.com/-MulBuBYT42s/UdxMJYAZynI/AAAAAAAAA38/ATfvnGvnRHg/s1600/mongolab1.jpg)[![](http://1.bp.blogspot.com/-Jj9YFU0NW4M/UdxMQvhCzkI/AAAAAAAAA4E/aqT1-MWHPmo/s320/mongolab2.jpg)](http://1.bp.blogspot.com/-Jj9YFU0NW4M/UdxMQvhCzkI/AAAAAAAAA4E/aqT1-MWHPmo/s1600/mongolab2.jpg) 
Now just confirm payment and voila - you have a replica set database, with up to 8GB storage! These replica sets run in Windows Azure Virtual Machines in either US East or US West data centers, so it's best to colocate your application in one of these data centers as well, to take advantage of MongoLab's hosted MongoDB service. 
If you need a larger database, you'll still need to go the self-host route, but if 8GB works for you, this is a very easy way to get up and running (since there's no database for you to install). 
For more information, check out MongoLab's [official blog post](http://blog.mongolab.com/2013/07/production-mongodb-replica-sets-now-available-on-windows-azure/)


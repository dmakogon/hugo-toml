+++
author = "David Makogon"
categories = ["Azure", "Crosspost", "Isv"]
date = 0001-01-01T00:00:00Z
description = ""
draft = false
slug = "cross_post_isv_guest_post_series_linx_powers_its_point_of_sale_systems_with_windows_azure"
tags = ["Azure", "Crosspost", "Isv"]
title = "Cross-post: ISV Guest Post Series: Linx Powers its Point-of-Sale Systems with Windows Azure"

+++


Fernando Chaves, e-Commerce Program Manager at , talks about their LinxWeb Point-of-Sale system that’s now running on Windows Azure. The full post is published on the Windows Azure blog, [here](http://blogs.msdn.com/b/windowsazure/archive/2012/06/27/isv-guest-post-series-linx-powers-its-point-of-sale-systems-with-windows-azure.aspx)

One of the interesting tidbits in this write-up is around the shift of media content to blob storage and CDN. Traditionally, Linx stored this content in their SQL Server database. This meant that, with every request for content, both the database server and IIS were taxed, handling the retrieval and streaming of content. Once their media was shifted to blob storage:

* They saw an approx. 75% reduction in database size.
* They saw significant load taken off their database and web servers, resulting in much faster response times on their servers due to reduced load. With content located in blobs (or CDN), web pages can simply link directly to this content, which completely bypasses IIS and the database server.

This post is one of several in the Windows Azure ISV Guest Post Series. The entire list is [here](http://www.davidmakogon.com/2012/04/look-at-windows-azure-isv-blog-series.html)


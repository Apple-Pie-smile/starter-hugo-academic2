---
url_pdf: ""
summary: Designed and implemented a stock matching machine to match buy and sell
  orders, use socket to receive information and parse xml, interact with
  PostgreSQL database, and return xml success/failure information.
url_video: ""
date: 2016-04-27T00:00:00Z
external_link: ""
url_slides: ""
title: Stock Matching with Scalibility
tags:
  - C++
  - PostgreSQL
  - XML
image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart
url_code: ""
---
Designed and developed a stock transaction system enabling users to create personal account and stock symbols, buy and sell orders, monitor order status etc. in C++

Applied socket programming to transmit XML requests/responses between client and server side in real-time

Implemented database schema in PostgreSQL to persist, manage and process account’s balance, shares and orders

Implemented priority queue data structure to manage client and server communication in multiple threads to handle high-concurrency requests and reduced the message delay time by 90%

Generated test cases on multi-threading modules and achieved more than 110 QPS per core based on the scalability validation
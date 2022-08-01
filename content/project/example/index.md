---
title: Stock Matching with Scalibility
summary: Designed and implemented a stock matching machine to match buy and sell orders, use socket to receive information and parse xml, interact with PostgreSQL database, and return xml success/failure information.
tags:
  - C++,PostgreSQL, XML
date: '2016-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---
Stock Matching with Scalibility| C++,PostgreSQL, XML, socket, multithread, concurrency
•	Designed and implemented a stock matching machine to match buy and sell orders, use socket to receive information and parse xml, interact with PostgreSQL database, and return xml success/failure information
•	Implemented functions such as creating account/stock symbols, creating buy/sell orders, matching orders, querying order status, etc.
•	Handled error cases such as wrong xml format input/operating on non-existing accounts/amount type is not a number/ID type is not a non-negative integer, etc.
•	For scalability, implement multithreading to connect to multiple clients, and ensure that the main thread exits after the child thread. In order to avoid too many threads, two queues are used, one records the client fd and xml information of the client in the socket, and the other takes messages from the queue for processing.
•	Used an atomic int variable to record the number of threads to ensure atomicity, and a concurrency queue to ensure the atomicity of each fetch operation. In order to avoid the concurrency of database reads and writes, it is locked before each operation and unlocked after each operation.
•	Wrote a random xml generator and a multi-threaded client to test the scalability of this project







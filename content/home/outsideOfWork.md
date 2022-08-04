---
widget: blank
widget_id: blank
headless: true
weight: 126
title: Outside of Work
subtitle: null
content:
  page_type: blank
design:
  columns: "2"
---


Accompany my cat Mochi

She's so sweet!

![](mochi.jpg)

{{ $image := resources.Get "media/mochi.jpg" }}
{{ $image := $image.Resize "600x400" }}
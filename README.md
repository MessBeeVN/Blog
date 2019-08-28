# Blog
Use
YAML Post Example:

---
layout: post
title:  "We all wait for summer"
author: john
categories: [ Jekyll, tutorial ]
image: assets/images/5.jpg
---
comments: false - disable comments in posts

image: "https://www.myexternal.com/image.jpg" - set external featured image

tags: [featured] - to display Featured posts on homepage

YAML Page Example:

---
title: "About"
permalink: "/about.html"
image: "/assets/images/screenshot.jpg"
---
Add sticky post on homepage

Tag a post as sticky to highlight a post on homepage.

Example:

---
layout: post
title:  "Could we reinvent the charm of old cities"
author: jane
categories: [ Jekyll, tutorial ]
image: assets/images/home.jpg
tags: [sticky]
---

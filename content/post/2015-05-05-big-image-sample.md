---
title: Test Post
subtitle: Using Multiple Images
date: 2021-04-05
tags: ["example", "bigimg"]
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}, {src: "/img/sphere.jpg", desc: "Sphere"}, {src: "/img/hexagon.jpg", desc: "Hexagon"}]
draft: true
---


A single bigimg can be specified in the front matter by the following YAML:
```
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}]
```
<!-- more -->
Multiple bigimgs can be specified in the front matter by the following YAML:
```
bigimg: [{src: "/img/triangle.jpg", desc: "Triangle"}, 
         {src: "/img/sphere.jpg", desc: "Sphere"}, 
         {src: "/img/hexagon.jpg", desc: "Hexagon"}]
```

Also note that the description field is optional, and images could instead be specified by:
```
bigimg: [{src: "/img/triangle.jpg"}, 
         {src: "/img/sphere.jpg"}, 
         {src: "/img/hexagon.jpg"}]
```

The above YAML array of hashes were written in "flow" style. However when generating a new page or post with `hugo new post/mypost.md`, hugo may interpret the archetype for bigimg in the default YAML style. Defining multiple bigimg's complete with descriptions in this style would be specified by:
```
bigimg: 
- {src: "/img/triangle.jpg", desc: "Triangle"}
- {src: "/img/sphere.jpg", desc: "Sphere"}
- {src: "/img/hexagon.jpg", desc: "Hexagon"}
```

Additional information can be found [in this YAML tutorial](https://rhnh.net/2011/01/31/yaml-tutorial/).

---
title: "Ова е наслов"
tagline: ""
header:
  overlay_image: https://i.imgur.com/Lt4ZTpF.png
  overlay_filter: 0.5
  teaser: /assets/images/500x300.png
  og_image: /assets/images/500x300.png
  caption: ""
categories:
  - Објава
tags:
  - протест
---

This post should display a **header with an overlay image** and **custom tagline**, if the theme supports it.

{% capture fig_img %}
![Foo]({{ "https://i.imgur.com/Lt4ZTpF.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>НАПРЕД!</figcaption>
</figure>

Non-square images can provide some unique styling issues.

This post tests overlay header images with custom `page.tagline`.

```yaml
tagline: "This is a custom tagline content which overrides the default page excerpt."
header:
  overlay_image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
```

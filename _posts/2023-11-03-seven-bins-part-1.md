---
title: "The Seven Bins of St Helens - Part 1"
date: 2023-11-03 00:00:00
tagline: "Are seven bins more effective than one? In this series of blog posts, I explore the answer to this question using public data on recycling rates by local authority in England."
header:
  overlay_image: "/assets/images/recycling.jpg"
  caption: "Photo by [SHVETS production](https://www.pexels.com/photo/woman-selecting-glass-into-plastic-container-7512859/)"
categories:
  - Environment
tags:
  - environment
  - data-analysis
  - tableau
---

In this series, I'm using public data to answer a question about recycling in England. Within this project I'll be accessing [open government data](https://www.data.gov.uk) and exploring options to gather data that isn't yet stored in a public database ([crowdsourcing](https://www.clickworker.com/customer-blog/data-crowdsourcing/) vs [freedom of information request](https://www.gov.uk/make-a-freedom-of-information-request/how-to-make-an-foi-request)).

#### Articles in this series

- [Seven Bins Part 1](/_posts/2023-11-03-seven-bins-part-1.md)
- [Seven Bins Part 2](/_posts/2023-11-16-seven-bins-part-2.md)
- [Seven Bins Part 3](/_posts/2024-02-10-seven-bins-part-3.md)

## Situation
Last week I took my son to visit my parents for the half-term break. They live in St Helens, a town in Merseyside, north-west England. One evening while I was there, the conversation turned to the new recycling bag that the council had just issued to every household in the borough. Despite our Prime Minister's recent promise that [he will never allow 'seven bins' per household](https://www.mrw.co.uk/news/government-will-never-allow-seven-bins-per-house-says-sunak-20-09-2023/), it seems that is exactly what [St Helens Borough Council is doing](https://www.sthelens.gov.uk/article/9028/Recycling-Service-Change). The new 70L green bag that my parents received brings their total household waste receptacle count to exactly seven:

- **Green bag** for cardboard
- **Blue bag** for paper
- **Black box** for glass
- **White bag** for plastic and cans
- **Grey caddy** for food waste
- **Green bin** for garden waste (a subscription service)
- **Brown bin** for general and non-recyclable waste

<div class="gallery" data-columns="1">
	<img src="/images/blog/2023-11-03-seven-bins-part-1/mums-bins-1.png">
	<img src="/images/blog/2023-11-03-seven-bins-part-1/mums-bins-2.png">
	<img src="/images/blog/2023-11-03-seven-bins-part-1/mums-bins-3.png">
</div>

This system of recycling, called [kerbside sort or multi-stream](https://en.wikipedia.org/wiki/Kerbside_collection#United_Kingdom), puts the burden of sorting the recyclable material on the resident. As my mum can attest, it is pretty onerous and sometimes confusing to work out what belongs in each bin or box, and when they each have to be put out for collection. In other parts of the UK, including in Waverley, where I live, the local authority employs a [co-mingled recycling](https://en.wikipedia.org/wiki/Single-stream_recycling) system, where all of the non-organic recyclable material is put into a single bin and the sorting takes place at a [Materials Recovery Facility](https://en.wikipedia.org/wiki/Materials_recovery_facility).

## Question
> Do councils who employ a kerbside sort system achieve higher recycling rates than those who employ the co-mingled system?

Mum and I looked up the latest recycling rates for Waverley and St Helens and were surprised to discover that St Helens, with its kerbside sort system, recycled just 36.8% of household waste in FY2021/22, compared to Waverley, with its co-mingled system, which achieved 58.9% in the same period (source: [Defra](https://www.gov.uk/government/statistical-data-sets/env18-local-authority-collected-waste-annual-results-tables-202122)).

In this series of blog posts, I intend to explore a fuller answer to this question using public data on recycling rates by local authority in England.

I do have some hypotheses on what I might find. On the one hand, having the waste sorted by the resident before collection may lead to less waste rejected for recycling, and thus improve the overall recycling rate. On the other hand, the burden of sorting and storing seven different bins may put householders off from doing any recycling and they may choose to put all of their waste, recyclable or not, in the brown bin.

Keep following to see where this exciting investigation leads!
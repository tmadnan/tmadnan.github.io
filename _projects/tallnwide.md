---
title: "TallnWide: Fast, Scalable and Geo-Distributed PCA for Big Data Analytics"
collection: projects
category: published
permalink: /projects/tallnwide-pca-bigdata
layout: single
author_profile: true
year: 2021
order: 8
publication: "Information Systems"
paperurl: "https://tmadnan10.github.io/files/pdf/research/tallnwide.pdf"
code: "https://github.com/tmadnan10/TallnWide"
---

We introduce **TallnWide**, a novel algorithm for performing Principal Component Analysis (PCA) on extremely large, high-dimensional datasets that are distributed across geographic locations, addressing both scalability and communication overhead in big data analytics. <!--more-->
- PCA is widely used for dimensionality reduction but faces scalability issues when both rows and columns grow large; existing methods can suffer from memory overflow and high communication cost in distributed environments. 
- TallnWide leverages a *zero-noise-limit Probabilistic PCA model* with a block-division strategy to manage **tall and wide data** efficiently, suppressing intermediate data explosion. 
- The algorithm introduces communication-efficient coordination among geographically distributed datacenters by transmitting only necessary parameters and minimizing idle computation time. 
- Empirical evaluation on real large-scale datasets shows TallnWide handles significantly higher dimensions (10× larger) and achieves up to **2.9× faster runtime** compared to conventional approaches in geo-distributed settings.  
- For reproducibility and future extension, TallnWide’s implementation is available as open-source, enabling further research in scalable dimension reduction on distributed data. 

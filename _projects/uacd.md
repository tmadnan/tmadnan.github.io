---
title: "UACD: User Attributed Core Decomposition for Influential Spreaders"
collection: projects
category: published
permalink: /projects/uacd-influential-spreaders
layout: single
author_profile: true
year: 2021
order: 7
publication: "Distributed Systems / Social Network Analytics"
paperurl: "https://tmadnan10.github.io/files/pdf/research/uacd.pdf"
---

We propose **User Attributed Core Decomposition (UACD)**, a novel graph analytic method that identifies the most influential spreaders in large social networks by combining network topology with rich user-specific information (followers, friends, tweet counts, verified status) in a distributed setting. UACD significantly improves accuracy and scalability over existing local and global centrality measures by incorporating both structural and user attributes. <!--more-->
- Introduced **UACN (User Attributed Core Number)**, a measure that augments traditional k-core decomposition with user features to better capture real influence potential.   
- Designed UACD to **use only local neighborhood information**, avoiding the prohibitive memory/runtime costs of global centrality measures on massive graphs.   
- Provided a **distributed implementation** of the algorithm on AWS EC2, demonstrating scalability to networks with tens of millions of nodes.   
- Empirically evaluated UACD against state-of-the-art spreader identification methods using standard metrics (e.g., Kendall τ, Spearman ρ, modified Jaccard similarity), showing **~12.5% higher accuracy** on average.   
- Achieved **up to 175× faster runtime** than global centrality approaches while maintaining high ranking quality across real Twitter datasets. 

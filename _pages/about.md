---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am an Applied Scientist II at Amazon Store Foundational AI, where I build foundation models and large language models for shopping search, retrieval, and recommendation. I received my Ph.D. from the Graduate Group in Applied Mathematics ([GGAM](http://appliedmath.ucdavis.edu/)) at UC Davis in March 2022.

My research centers on reinforcement learning and policy optimization for large language models, and on stochastic and zeroth-order optimization.

You can find me on [Google Scholar](https://scholar.google.com/citations?hl=en&user=40szSMwAAAAJ), [OpenReview](https://openreview.net/profile?id=~Zhongruo_Wang2), and [LinkedIn](https://www.linkedin.com/in/zhongruo-wang-a24a5078/).

Experience
======
At Amazon Store Foundational AI, I have worked on:

* **2022–2023** — RoBERTa-based behavior foundation models and graph models for search/ads retrieval and recommendation.
* **2024** — Instruction-following LLM-based embedding models for retrieval and recommendation.
* **2024** — Generative recommender for customer representation (Synergen).
* **2025** — Small language model pretraining, midtraining, and post-training (on-policy distillation, RLVR) for shopping generative tasks such as query rewrite, final-stage ranking, and shopping mission generation.
* **2025** — Foundation model post-training on user behavior data.
* **2026** — Personalized search agent for user-context retrieval, based on SQL and semantic search.

Publications
======
{% if site.author.googlescholar %}You can also find my articles on my <a href="{{site.author.googlescholar}}">Google Scholar profile</a>.{% endif %}

{% for category in site.publication_category %}
{% assign title_shown = false %}
{% for post in site.publications reversed %}
{% if post.category != category[0] %}{% continue %}{% endif %}
{% unless title_shown %}
<h2 id="{{ category[0] }}" class="archive__subtitle">{{ category[1].title }}</h2>
{% assign title_shown = true %}
{% endunless %}
{% include archive-single.html %}
{% endfor %}
{% endfor %}

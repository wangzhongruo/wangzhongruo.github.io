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

Selected Citations
======
My paper *Zeroth-Order Algorithms for Nonconvex-Strongly-Concave Minimax Problems with Improved Complexities* (Journal of Global Optimization, 2022) has been cited by work published at top machine learning venues, including **NeurIPS** (6), **AISTATS** (4), **ICML** (3), **ICLR** (3), and **JMLR** (2) — 18 citations across these venues to date.

| Year | Venue | Citing paper |
|------|-------|--------------|
| 2026 | NeurIPS | PaZO: Preconditioned Accelerated Zeroth-Order Optimization for Fine-Tuning LLMs |
| 2026 | NeurIPS | Bilevel ZOFO: Efficient LLM Fine-Tuning and Meta-Training |
| 2026 | NeurIPS | Stochastic Regret Guarantees for Online Zeroth- and First-Order Bilevel Optimization |
| 2026 | JMLR | A Fully Parameter-Free Second-Order Algorithm for Convex-Concave Minimax Problems |
| 2026 | AISTATS | ConMeZO: Adaptive Descent-Direction Sampling for Gradient-Free Finetuning of Large Language Models |
| 2025 | NeurIPS | Zeroth-Order Optimization Finds Flat Minima |
| 2025 | ICLR | Adversarial Machine Unlearning |
| 2025 | ICLR | Second-Order Fine-Tuning without Pain for LLMs: A Hessian-Informed Zeroth-Order Optimizer (HiZOO) |
| 2024 | NeurIPS | Robust and Faster Zeroth-Order Minimax Optimization: Complexity and Applications |
| 2024 | ICML | Gradient-Free Method for Heavily Constrained Nonconvex Optimization |
| 2024 | ICLR | Addax: Utilizing Zeroth-Order Gradients to Improve Memory Efficiency and Performance of SGD for Fine-Tuning Language Models |
| 2023 | NeurIPS | Fine-Tuning Language Models with Just Forward Passes (MeZO) |
| 2023 | ICML | DPZero: Private Fine-Tuning of Language Models without Backpropagation |
| 2023 | ICML | Communication-Efficient Federated Hypergradient Computation via Aggregated Iterative Differentiation |
| 2023 | AISTATS | Stochastic Gradient Descent-Ascent: Unified Theory and New Efficient Methods |
| 2023 | AISTATS | No-regret Sample-Efficient Bayesian Optimization for Finding Nash Equilibria with Unknown Utilities |
| 2021 | AISTATS | AdaGDA: Faster Adaptive Gradient Descent Ascent Methods for Minimax Optimization |
| 2020 | JMLR | Accelerated Zeroth-Order and First-Order Momentum Methods from Mini to Minimax Optimization |

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

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

Research Impact
======
My research spans the post-training of large language models with reinforcement learning and the optimization theory that underlies modern machine learning.

**Large language model post-training and reinforcement learning (RLVR).** My recent work develops post-training methods for large language models, spanning supervised fine-tuning and reinforcement learning with verifiable rewards (RLVR). Representative contributions include *SFT Doesn't Always Hurt General Capabilities* (ICLR 2025), which characterizes when domain-specific fine-tuning preserves versus erodes a model's general ability; *ST-PPO: Stabilized Off-Policy Proximal Policy Optimization for Multi-Turn Agents Training* (COLM 2026), for training multi-turn LLM agents; *Reward-Wise Value Estimation for Multi-Reward Optimization in LLMs* (ICML 2026); and *Reinforcement Learning in Inference Time: A Perspective from Successive Policy Iterations* (NeurIPS 2025). In applied settings, these methods support small-language-model pretraining and post-training — on-policy distillation and RLVR — for large-scale shopping generative tasks such as query rewriting and ranking.

My first-authored paper *Zeroth-Order Algorithms for Nonconvex-Strongly-Concave Minimax Problems with Improved Complexities* (Journal of Global Optimization, 2022; earlier NeurIPS 2020 Workshop and arXiv versions) develops derivative-free (zeroth-order) algorithms with improved iteration and query complexity for nonconvex-strongly-concave minimax problems, where gradients are unavailable and only function evaluations can be queried. Cited across its versions by work at NeurIPS, ICML, ICLR, JMLR, AISTATS, TMLR, and SIAM Journal on Optimization, it has contributed to two further lines of research.

**Min-max optimization theory.** The paper's complexity analysis and single-loop zeroth-order scheme are a building block for nonconvex saddle-point theory, extended by later work on single-loop algorithms without strong concavity ([AISTATS 2022](https://proceedings.mlr.press/v151/yang22b.html)), duality-gap and Polyak–Łojasiewicz rates ([JMLR](https://www.jmlr.org/papers/volume24/21-1471/21-1471.pdf), [2023](https://jmlr.org/papers/v24/22-1518.html)), Nash-equilibrium search and derivative-free projection methods (SIAM Journal on Optimization [2021](https://epubs.siam.org/doi/10.1137/20M1337600), [2024](https://epubs.siam.org/doi/10.1137/23M1568168)), and robust zeroth-order minimax methods (NeurIPS 2024).

**Zeroth-order LLM training.** The paper's core idea — estimating descent directions from forward evaluations alone, without backpropagation — now underpins memory-efficient LLM fine-tuning, and it is cited by MeZO ([NeurIPS 2023](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a627810151be4d13f907ac898ff7e948-Abstract-Conference.html)), DPZero (ICML 2023), Addax (ICLR 2024), HiZOO (ICLR 2025), MUZO ([EMNLP 2025](https://aclanthology.org/2025.emnlp-main.432/)), and PaZO (NeurIPS).

Representative citing work across its NeurIPS 2020 Workshop, arXiv, and journal versions (NeurIPS, ICML, ICLR, JMLR, AISTATS, TMLR, SIAM Journal on Optimization, EMNLP, and IJCAI):

| Year | Venue | Citing paper |
|------|-------|--------------|
| 2026 | NeurIPS | PaZO: Preconditioned Accelerated Zeroth-Order Optimization for Fine-Tuning LLMs |
| 2026 | NeurIPS | Bilevel ZOFO: Efficient LLM Fine-Tuning and Meta-Training |
| 2026 | NeurIPS | Stochastic Regret Guarantees for Online Zeroth- and First-Order Bilevel Optimization |
| 2026 | AISTATS | ConMeZO: Adaptive Descent-Direction Sampling for Gradient-Free Finetuning of Large Language Models |
| 2026 | JMLR | A Fully Parameter-Free Second-Order Algorithm for Convex-Concave Minimax Problems |
| 2025 | NeurIPS | Zeroth-Order Optimization Finds Flat Minima |
| 2025 | ICLR | Adversarial Machine Unlearning |
| 2025 | ICLR | Second-Order Fine-Tuning without Pain for LLMs: A Hessian-Informed Zeroth-Order Optimizer (HiZOO) |
| 2025 | EMNLP | MUZO: Leveraging Multiple Queries and Momentum for Zeroth-Order Fine-Tuning of Large Language Models |
| 2025 | IJCAI | Sharpness-Aware Zeroth-Order Optimization for Graph Transformers |
| 2025 | TMLR | Min-Max Optimisation for Nonconvex-Nonconcave Functions Using a Random Zeroth-Order Extragradient Algorithm |
| 2025 | TMLR | A Framework for Finding Local Saddle Points in Two-Player Zero-Sum Black-Box Games |
| 2024 | NeurIPS | Robust and Faster Zeroth-Order Minimax Optimization: Complexity and Applications |
| 2024 | ICML | Delving into the Convergence of Generalized Smooth Minimax Optimization |
| 2024 | ICLR | Addax: Utilizing Zeroth-Order Gradients to Improve Memory Efficiency and Performance of SGD for Fine-Tuning Language Models |
| 2024 | SIAM J. Opt. | Derivative-Free Alternating Projection Algorithms for General Nonconvex-Concave Minimax Problems |
| 2023 | NeurIPS | Fine-Tuning Language Models with Just Forward Passes (MeZO) |
| 2023 | NeurIPS | SimFBO: Towards Simple, Flexible and Communication-Efficient Federated Bilevel Learning |
| 2023 | ICML | DPZero: Private Fine-Tuning of Language Models without Backpropagation |
| 2023 | ICML | Communication-Efficient Federated Hypergradient Computation via Aggregated Iterative Differentiation |
| 2023 | AISTATS | Stochastic Gradient Descent-Ascent: Unified Theory and New Efficient Methods |
| 2023 | AISTATS | No-regret Sample-Efficient Bayesian Optimization for Finding Nash Equilibria with Unknown Utilities |
| 2023 | JMLR | Fast Objective & Duality Gap Convergence for Nonconvex-Strongly-Concave Min-Max Problems with PL Condition |
| 2023 | JMLR | Zeroth-Order Alternating Gradient Descent Ascent Algorithms for a Class of Nonconvex-Nonconcave Minimax Problems |
| 2022 | ICML | Gradient-Free Method for Heavily Constrained Nonconvex Optimization |
| 2022 | AISTATS | Faster Single-Loop Algorithms for Minimax Optimization without Strong Concavity |
| 2022 | AISTATS | Zeroth-Order Methods for Convex-Concave Min-Max Problems: Applications to Decision-Dependent Risk Minimization |
| 2022 | SIAM J. Opt. | New First-Order Algorithms for Stochastic Variational Inequalities |
| 2021 | NeurIPS | Global Convergence to Local Minmax Equilibrium in Classes of Nonconvex Zero-Sum Games |
| 2021 | AISTATS | Direct-Search for a Class of Stochastic Min-Max Problems |
| 2021 | AISTATS | AdaGDA: Faster Adaptive Gradient Descent Ascent Methods for Minimax Optimization |
| 2021 | SIAM J. Opt. | Efficient Search of First-Order Nash Equilibria in Nonconvex-Concave Smooth Min-Max Problems |
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

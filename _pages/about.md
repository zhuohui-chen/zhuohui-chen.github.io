---
permalink: /
title: "Hihaody 👋"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I'm Zhuohui (Jerry) Chen, a third-year Ph.D. student at the [College of Information, University of Maryland, College Park](https://ischool.umd.edu/), advised by Prof. Zubin Jelveh. I study how to make large language models **trustworthy enough for high-stakes decisions**: secure as agents, reliable as judges and annotators, and useful as forecasters.

Before my Ph.D., I spent three years as a Research Analyst in the Central Bank Operations Division of the [International Monetary Fund](https://www.imf.org/)'s Monetary and Capital Markets Department. There I built forecasting models that central banks use, co-authored IMF working papers on tail-risk and reserve-demand forecasting, and joined 25+ technical assistance and financial sector assessment missions. My background is unusually mixed: computer science, English and translation studies, and public administration. That mix is why I care about language, measurement, and real-world use in equal parts.

<div class="notice--info" markdown="1">
**I'm looking for research internships for Summer 2027**, especially in LLM agents, evaluation, and AI for finance or forecasting. Feel free to [email me](mailto:zchen95@umd.edu) or see my [CV (PDF)](https://drive.google.com/file/d/1CPSGyz5djb9XpP3v9VmcuijJ3RrgaYgX/view?usp=sharing).
</div>

## Research

My current work follows three connected threads:

- **LLMs for forecasting and judgment.** Can LLM agents make *judgmental* forecasts, the kind human experts make by combining models, data, and context? I'm building an agentic framework to study this, drawing on my forecasting work at the IMF.
- **Trustworthy and secure LLM agents.** Agents that read tool outputs, web pages, and documents can be hijacked by prompt injection. I study detectors that use the model's own internal signals, and alignment methods that hold up when preference data is poisoned.
- **LLMs as measurement instruments.** When social scientists use LLMs to code or annotate text, how far can we trust the labels? I use controlled synthetic data and human-annotation benchmarks to find where LLM coders succeed and where they fail.

I also work on multilingual and code-switched NLP, including pragmatic realism in synthetic code-switched data and catastrophic forgetting during code-switched fine-tuning. More on the [Research](/research/) page.

## News

<ul class="news">
  <li><span class="news__date">2026</span> Received the Do Good Accelerator Fellowship for the second year.</li>
  <li><span class="news__date">Dec 2025</span> Finished <em>Huber DPO</em>, a robust DPO loss that resists poisoned preference data.</li>
  <li><span class="news__date">2025</span> Received the Do Good Accelerator Fellowship.</li>
  <li><span class="news__date">Oct 2024</span> IMF handbook chapter <a href="/publication/liquidity-forecasting-part-ii"><em>Liquidity Forecasting—Part II: The Statistical Component</em></a> published.</li>
  <li><span class="news__date">Sep 2024</span> Started my Ph.D. at UMD with a Dean's Fellowship.</li>
  <li><span class="news__date">Jul 2024</span> Our reserve-demand model was used in Box 7 of the IMF's <a href="/publication/us-article-iv-2024">2024 U.S. Article IV report</a> to size the Fed's reserve needs.</li>
  <li><span class="news__date">May 2024</span> IMF Working Paper <a href="/publication/forecasting-tail-risk"><em>Forecasting Tail Risk via Neural Networks with Asymptotic Expansions</em></a> released.</li>
  <li><span class="news__date">Sep 2023</span> IMF Working Paper <a href="/publication/modeling-reserve-demand"><em>Modeling the Reserve Demand to Facilitate Central Bank Operations</em></a> released and presented at the 2023 International Symposium on Forecasting.</li>
</ul>

## Selected work

{% assign selected = "forecasting-tail-risk,modeling-reserve-demand,liquidity-forecasting-part-ii" | split: "," %}
{% for slug in selected %}
  {% assign target = "/publication/" | append: slug %}
  {% for post in site.publications %}
    {% if post.url == target %}{% include pub-entry.html %}{% endif %}
  {% endfor %}
{% endfor %}

[All publications →](/publications/)

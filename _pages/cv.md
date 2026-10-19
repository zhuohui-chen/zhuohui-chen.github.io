---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<p class="page-lead">Email <a href="mailto:zchen95@umd.edu">zchen95@umd.edu</a> · <a href="https://github.com/zhuohui-chen">GitHub</a> · <a href="{{ site.author.googlescholar }}">Google Scholar</a> · <a href="{{ site.author.orcid }}">ORCID</a></p>

<p><a class="pill pill--lg" href="https://drive.google.com/file/d/1CPSGyz5djb9XpP3v9VmcuijJ3RrgaYgX/view?usp=sharing">Download CV (PDF)</a></p>

## Research interests

LLMs for forecasting and finance · Trustworthy and secure LLM agents · LLM evaluation and LLM-as-a-judge · Data-centric AI and computational social science · Multilingual NLP

## Education

<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>University of Maryland, College Park</strong></span><span>2024–present</span></div>
  Ph.D. in Information Science · GPA 4.0/4.0 · Dean's Fellowship<br>
  <span class="cv-entry__detail">Coursework: Natural Language Processing, Generative AI Agents, Long-Context Language Models, Multilingual LLMs, Commonsense Reasoning and NLU, Advanced Machine Learning, Constructivist Grounded Theory</span>
</div>
<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>University of Maryland, College Park</strong></span><span>2019–2020</span></div>
  Master of Public Administration · GPA 3.94/4.0
</div>
<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>Guangdong University of Foreign Studies</strong></span><span>2017–2020</span></div>
  M.A. in Translation Studies · GPA 92/100
</div>
<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>Guangdong University of Technology</strong></span><span>2013–2017</span></div>
  B.S. in Computer Science; B.A. in English for Science and Technology · GPA 3.99/4.0
</div>

## Experience

<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>International Monetary Fund</strong>, Monetary and Capital Markets Department</span><span>2021–2024</span></div>
  <em>Research Analyst, Central Bank Operations Division</em>
  <ul>
    <li>Co-developed CoFiE-NN, an LSTM with Cornish–Fisher expansions for Value-at-Risk forecasting that outperformed EGARCH-t and EVT across 22 currencies; built the backtesting framework.</li>
    <li>Built a reserve-demand model (WP/23/179) used in the IMF's 2024 U.S. Article IV report to estimate the Fed's reserve needs (US$2.1–3.2 trillion).</li>
    <li>Developed and taught Python/R/MATLAB liquidity-forecasting tools delivered to 15+ central banks; first-authored the IMF handbook chapter on their statistical methods.</li>
    <li>Joined 25+ technical assistance and FSAP missions, including stress testing of liquidity, solvency, and interconnectedness for Saudi Arabia and Panama.</li>
    <li>Automated extraction of Bank of Japan securities-operations data from PDFs and the web.</li>
  </ul>
</div>
<div class="cv-entry">
  <div class="cv-entry__head"><span><strong>United Nations Development Programme</strong>, Bureau for Policy and Programme Support</span><span>2020–2021</span></div>
  <em>Policy Analyst Intern</em>
  <ul>
    <li>Compiled and analyzed economic and sovereign debt data for 136 countries, producing simulations, charts, and tables for policy research.</li>
    <li>Built a global COVID-19 vaccine administration and cost dataset and estimated country-level spending under multiple scenarios.</li>
    <li>Contributed analysis and policy interpretation to research papers and policy briefs.</li>
  </ul>
</div>

## Research projects

See the [Research](/research/) page for details.

- **TimeJudge: An Agentic Framework for Judgmental Forecasting** (in progress)
- **Robust Attention Shield for Prompt Injection** (in progress)
- **LLM Deductive Coding with Controlled Synthetic Data** (in progress)
- Huber DPO: A Robust Framework for LLM Alignment (course project, 2025)
- Towards Pragmatic Realism in Synthetic Code-Switched Data (course project)
- Containing Catastrophic Forgetting in Code-Switched Multitask Continual Fine-tuning (course project)
- Lost in Translation: Stress-Testing Greater Chinese Cultural and Pragmatic Nuance (course project)
- Demojification of Online Social Biases (course project)

## Publications

{% for category in site.publication_category %}
<h3 class="cv-subhead">{{ category[1].title }}</h3>
{% assign pubs = site.publications | sort: "date" | reverse %}
{% for post in pubs %}{% if post.category == category[0] %}{% include pub-entry.html %}{% endif %}{% endfor %}
{% endfor %}

## Teaching

{% assign courses = site.teaching | sort: "date" | reverse %}
<ul>
{% for post in courses %}
  <li><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>, <em>{{ post.type }}</em>, {{ post.date | date: "%Y" }}</li>
{% endfor %}
</ul>

## Honors and awards

<div class="cv-list">
  <div><span>Do Good Accelerator Fellowship</span><span>2025, 2026</span></div>
  <div><span>Dean's Fellowship, University of Maryland</span><span>2024</span></div>
  <div><span>Scholarship for International Organization Internship</span><span>2021</span></div>
  <div><span>Overseas Study Scholarship</span><span>2019</span></div>
  <div><span>Graduated with Honors</span><span>2017</span></div>
  <div><span>China National Scholarship</span><span>2014, 2016</span></div>
  <div><span>First Tier Scholarship</span><span>2014–2019</span></div>
</div>

## Skills

<div class="cv-list cv-list--skills">
  <div><span><strong>Programming</strong></span><span>Python, R, C++, Java, SQL, MATLAB, Stata</span></div>
  <div><span><strong>ML and data</strong></span><span>PyTorch, Hugging Face Transformers, scikit-learn, pandas, NumPy</span></div>
  <div><span><strong>Tools</strong></span><span>Git, Linux, Jupyter, LaTeX</span></div>
</div>

## Membership

Pi Alpha Alpha, 2020–present

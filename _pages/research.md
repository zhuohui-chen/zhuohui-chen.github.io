---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

My research asks when we can trust large language models with high-stakes judgment: as **forecasters**, as **autonomous agents**, and as **annotators and judges** of text. It also draws on earlier work in applied forecasting and financial stability at the IMF, and on multilingual NLP.

## Current projects

<div class="project">
<div class="project__head"><span class="project__title">TimeJudge: An Agentic Framework for Judgmental Forecasting</span><span class="tag tag--ongoing">In progress</span></div>
<p class="project__meta">Pre-candidacy independent research · expected Dec 2026</p>

Human experts rarely forecast with a model alone. They adjust statistical forecasts using news, context, and experience, a practice called <em>judgmental forecasting</em>. TimeJudge asks whether LLM agents can take on this role, and what it takes for their judgments to be reliable. Data collection, the agent framework, and the experiment design are complete.
</div>

<div class="project">
<div class="project__head"><span class="project__title">Robust Attention Shield for Prompt Injection</span><span class="tag tag--ongoing">In progress</span></div>
<p class="project__meta">Trustworthy and secure LLM agents</p>

LLM agents read untrusted content such as tool outputs, web pages, and emails, which attackers can use to inject instructions. This project studies how to detect such injections from the model's own attention signals. We benchmark training-free and learned detectors under a controlled protocol, covering direct prompt injection, injected tool responses, and multi-round agent tasks. We then analyze where and why they fail, as a basis for a more robust detector.
</div>

<div class="project">
<div class="project__head"><span class="project__title">LLM Deductive Coding with Controlled Synthetic Data</span><span class="tag tag--ongoing">In progress</span></div>
<p class="project__meta">LLMs as measurement instruments</p>

Social scientists increasingly use LLMs to code text against predefined categories. We study how reliable those codes are, using synthetic economics abstracts whose topic composition is known by construction, together with a human-annotation benchmark. Our analysis suggests that many apparent LLM "errors" are emergent topics the coding scheme did not anticipate. A pilot annotation study is complete, and the main human-annotation study is under way.
</div>

## Past research at the IMF (2021–2024)

<div class="project">
<div class="project__head"><span class="project__title">Forecasting Tail Risk with Neural Networks</span></div>

CoFiE-NN combines an LSTM with Cornish–Fisher expansions to forecast Value-at-Risk while keeping the outputs interpretable. It outperformed EGARCH-t and Extreme Value Theory models on simulated data and across 22 currencies. I built the cross-validation and backtesting framework (log score, interval score, Kupiec and Christoffersen tests, Lopez loss).
<span class="project__links"><a class="pill" href="/publication/forecasting-tail-risk">IMF WP/24/99</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Reserve Demand Modeling for Central Banks</span></div>

A framework for estimating how much central bank reserves the banking system demands at a given interest rate, comparing parametric sigmoid curves with machine-learning estimators. IMF staff used it in the 2024 U.S. Article IV report to estimate the reserves needed for the Federal Reserve's ample-reserves regime.
<span class="project__links"><a class="pill" href="/publication/modeling-reserve-demand">IMF WP/23/179</a><a class="pill" href="/publication/us-article-iv-2024">2024 U.S. Article IV, Box 7</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Liquidity Forecasting Framework for Central Bank Operations</span></div>

Statistical tools in Python, R, and MATLAB that forecast the autonomous factors driving systemic liquidity and banks' demand for reserves. The tools have been delivered to more than 15 central banks, and I taught their use in IMF training courses. I first-authored the IMF handbook chapter documenting the methods, and applied them in technical assistance such as the Guatemala mission.
<span class="project__links"><a class="pill" href="/publication/liquidity-forecasting-part-ii">Handbook chapter</a><a class="pill" href="/publication/guatemala-liquidity-forecasting">Guatemala TA report</a><a class="pill" href="/teaching/">Courses</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Financial Sector Assessment and Stress Testing</span></div>

Supported Financial Sector Assessment Programs with stress testing and modeling of liquidity, solvency, and interconnectedness risks.
<span class="project__links"><a class="pill" href="/publication/saudi-arabia-fsap">Saudi Arabia FSAP</a><a class="pill" href="/publication/panama-fsap">Panama FSAP</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Text Classification for Central Bank Legislation</span></div>

Implemented and compared eight Naive Bayes classifiers that sort segments of central bank legislation into thematic categories. This work fed a topic-recommendation module for the IMF's Central Bank Legislation Database.
</div>

## Course projects (Ph.D.)

<div class="project">
<div class="project__head"><span class="project__title">Huber DPO: A Robust Framework for LLM Alignment</span><span class="project__meta-inline">Dec 2025</span></div>
<p class="project__meta">with Yancheng Zhu and Zhaojun Xie</p>

Direct Preference Optimization is vulnerable to poisoned preference data. Huber DPO borrows from the statistical Huber loss to down-weight pairs with extreme reward margins, and adds a context-stability check that flags backdoor-poisoned pairs. It needs no external verifier and makes no assumption about the attack. It matched or beat vanilla and robust DPO baselines under random label flips, targeted attacks, and backdoor attacks. We also showed that backdoors can collapse standard DPO models into incoherent output.
</div>

<div class="project">
<div class="project__head"><span class="project__title">Towards Pragmatic Realism in Synthetic Code-Switched Data</span></div>
<p class="project__meta">with Samuel Miller and Ethan Baker · CMSC848T</p>

Synthetic code-switched text is usually judged on grammar alone. P-SwitchLingua adds two pragmatic dimensions: whether a switch happens in a plausible discourse context (*placement realism*) and whether it serves a plausible communicative function (*function realism*). We trained realism rankers on Chinese–English data, tested their transfer to Turkish–English and Telugu–English, and measured how well LLM-as-a-judge scores agree with these distributional measures. The pragmatically grounded pipeline produced data closer to natural code-switching, especially in where switches occur, and gained in function realism when paired with a refinement step. The LLM judge and the distributional rankers turned out to capture related but distinct notions of realism.
<span class="project__links"><a class="pill" href="https://github.com/zhuohui-chen/pragmatically_grounded_cos">Code</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Containing Catastrophic Forgetting in Code-Switched Multitask Continual Fine-tuning</span></div>
<p class="project__meta">with Meiyu Li, Quan Nguyen, Harshit Soora, and Claire O'Connor</p>

A multilingual model is adapted step by step to new code-switched languages (English → Chinese → Vietnamese → Hindi) and new tasks (reading comprehension → knowledge QA → natural language inference), with little old data available. We confirmed catastrophic forgetting under vanilla continual fine-tuning, and showed that adapters combined with limited replay and knowledge distillation reduce it.
<span class="project__links"><a class="pill" href="https://github.com/zhuohui-chen/code_switch_model">Code</a></span>
</div>

<div class="project">
<div class="project__head"><span class="project__title">Lost in Translation: Stress-Testing Greater Chinese Cultural and Pragmatic Nuance</span></div>
<p class="project__meta">with Jeremy Sha, Spencer Jenkins, and Amadeo Parra</p>

How well do LLMs preserve culture-specific meaning when translating Chinese and Cantonese? We built test sets for fine-grained kinship terms, Cantonese euphemisms, and emotion-carrying sentence-final particles, and evaluated translation in both directions with English and Spanish. Most models collapse detailed kinship terms into generic labels. Emotion is usually preserved, but often without the particle that originally carried it.
</div>

<div class="project">
<div class="project__head"><span class="project__title">Demojification of Online Social Biases</span></div>
<p class="project__meta">with Ziyang Chen and Yingzhen Cao</p>

Hate speech often hides behind emojis. We built a large emoji-cloaked dataset by systematically perturbing the Social Bias Inference Corpus with emoji swaps for verbs, identities, and slurs, positive-emoji confounders, and leetspeak, and audited it by hand. A fine-tuned RoBERTa outperformed GPT-4o-mini at detecting emoji-based hate.
</div>

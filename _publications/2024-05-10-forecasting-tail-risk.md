---
title: "Forecasting Tail Risk via Neural Networks with Asymptotic Expansions"
collection: publications
category: papers
permalink: /publication/forecasting-tail-risk
date: 2024-05-10
authors: 'Yuji Sakurai, <b>Zhuohui Chen</b>'
venue: 'IMF Working Paper WP/24/99'
excerpt: 'CoFiE-NN combines an LSTM with Cornish–Fisher expansions to forecast Value-at-Risk. It captures nonlinear dynamics in higher moments while keeping the output interpretable, and outperforms EGARCH-t and Extreme Value Theory models on simulated data and on 22 currencies.'
featured_link:
  name: 'IMF page'
  url: 'https://www.imf.org/en/Publications/WP/Issues/2024/05/10/Forecasting-Tail-Risk-via-Neural-Networks-with-Asymptotic-Expansions-548841'
links:
  - name: 'IMF page'
    url: 'https://www.imf.org/en/Publications/WP/Issues/2024/05/10/Forecasting-Tail-Risk-via-Neural-Networks-with-Asymptotic-Expansions-548841'
  - name: 'PDF'
    url: 'https://www.imf.org/-/media/files/publications/wp/2024/english/wpiea2024099-print-pdf.pdf'
citation: 'Sakurai, Y., and Chen, Z. (2024). &quot;Forecasting Tail Risk via Neural Networks with Asymptotic Expansions.&quot; <i>IMF Working Paper</i> No. 2024/099. International Monetary Fund.'
---

**Abstract.** We propose a new machine-learning-based approach for forecasting Value-at-Risk (VaR) named CoFiE-NN, where a neural network (NN) is combined with Cornish–Fisher expansions (CoFiE). CoFiE-NN can capture non-linear dynamics of high-order statistical moments thanks to the flexibility of a NN while maintaining interpretability of the outputs by using CoFiE, which is a well-known statistical formula. First, we explain CoFiE-NN. Second, we compare the forecasting performance of CoFiE-NN with three conventional models using both Monte Carlo simulation and real data. To do so, we employ Long Short-Term Memory (LSTM) as our main specification of the NN. We then apply CoFiE-NN to different asset classes, with a focus on foreign exchange markets. We report that CoFiE-NN outperforms the conventional EGARCH-t model and the Extreme Value Theory model in several statistical criteria for both the simulated data and the real data. Finally, we introduce a new empirical proxy for tail risk named tail risk ratio under CoFiE-NN. We discover that only 20 percent of tail risk dynamics across 22 currencies is explained by one common factor. This contrasts with the fact that 60 percent of volatility dynamics across the same currencies is explained by one common factor.

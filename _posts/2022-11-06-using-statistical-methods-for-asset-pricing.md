---
layout: post
title: "Using Statistical Methods For Asset Pricing"
categories: [data, markets]
date: 2022-11-06 17:22 -0400
---

Can asset prices be somewhat accurately estimated using statiscal methodologies a la Renaissance Technologies? The idea that mathematics and large amounts of computing power can be used to profitably participate in markets is not a new idea, but it is also not a generally accepted consensus. Computer-driven trading has been the attributed cause to several market events, usually crashes involving automated trading systems continuously selling based on signals produced by other automated systems. Financial intuition would say accurately pricing equities or other assets with many qualitative factors is unlikely or outright impossible for purely quantitative measures to capture. However, as machines become more capable with larger amounts of increasingly more qualitative data, the prospect of algorithmic trading systems seems more probable than ever.

Months ago, in early 2022, I used Keras and Tensorflow to predict digital asset prices with data I collected from Kraken's API. My reasoning for starting this project was out of curiosity regarding the validity of technical analysis, especially for assets that have scarce fundamentals. The results were not astounding, but the predicitions were far more accurate than I had anticipated. Perhaps using other nonlinear approximators on large finanical datasets could yield similar if not better results. I decided that I was not giving my model a fair chance, as it was trying to predict an exact price in the t+1 interval using associations learned from t data. The immediate improvement I came up with was to transform the problem from regression to classification, and defining return bins based off the volatility of the asset in question, but this would still restrict the model to a single asset.

In the near future, I am seeking to improve the current model that has been applied to digital assets. When I feel that significant progress has been made, I will attempt to translate these principles towards pricing commodity derivatives and potentially equities. Over the lifespan of this endeavour, I will try to maintain timely updates on progress and code samples so my work can be assessed and scrutinized. For those who may stumble across my journey to create my own pricing model, I hope something can be learned from my failures and hopefully that more can be learned from any successes. I cannot determine a timeline at this moment, but I am looking to prioritize this project over my other projects in my free time, which is already relatively scarce. I will still be posting current event articles when I have a chance, and I hope to come with updates soon.

Best,
Michael
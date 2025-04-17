---
tags: internet projects
title: meow_d LLM, v1
---

!["once Cohost ends I will fine-tune an an LLM on all my posts + my notes, creating the first ever LLM dedicated to posting cringe"](/assets/images/post-images/cringe-llm.png)

[link to some AI slop it generated.](/ai-slop)

dataset is acquired from my posts.json in my cohost-dl downloads, only because i already had it downloaded. it's probably better to only use the official data export, which only contains your own posts for legal reasons.

data preprocessing is done with python:
- get rid of shares, which can be identified as their `["astmap"]["spans"]` are empty
- get rid of all the data except for your title and post itself (`"headline"` and `"plainTextBody"`)

then format the dataset. can be done in different ways:
- human: "write a cohost post", assistant: title + post
- no prompt template, just title + post

choosing the model:
- "open source" models
  - when it comes to machine learning, the main bottleneck is vram, and training uses more vram than running.
  - train using unsloth, axoltol, etc
  - if you have a beefy computer or is using a relatively small model, you can just train on there. if you don't, use Google Colab or any other service out there.
- proprietary models
  - you'll only be able to use their proprietary services to train
  - example: Google AI studio

(written months ago i forgot about this so might as well put it out there. im too lazy to make it good)

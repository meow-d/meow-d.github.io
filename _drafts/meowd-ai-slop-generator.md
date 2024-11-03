I kept my promise. I've created the cringe generator.

!["once Cohost ends I will fine-tune an an LLM on all my posts + my notes, creating the first ever LLM dedicated to posting cringe"](/assets/images/post-images/cringe-llm.png)

[here's link of some AI slop it generated.](/secret/ai-slop.md)

- dataset acquired with cohost-dl
  - i used the posts.json from my cohost-dl download, only because i already had it downloaded. it's not the best for this use case as it doesn't just download your post - it downloads every single post you've ever liked and shared, including media. a better alternative would be the official data export, which only contains your own posts for legal reasons.

- data preprocessing with python cause i like python
  - the cohost-dl posts.json contains shares you'd want to get rid of, which can be identifyed as their `["astmap"]["spans"]` are empty
  - next you'll want to get rid of all the data except for your title and post itself (`"headline"` and `"plainTextBody"`)
  - convert to csv because everyone used csv

- ways you can format the dataset
  - title as input, post as output
  - "write a cohost post" as input, title + post as output
    - probably the best option
  - no input, just title + post as output
    - turns it into a general slop generator that you can't converse with

- where to train, and which model
  - "open source" models
    - when it comes to machine learning, the main bottleneck is vram. as a rule of thumb, training uses more vram than running. choose a model based on the vram available.
    - if you have a beefy computer, you can just train on there.
    - if you don't, use Google Colab, or any other service out there.
  - proprietary models
    - you'll only be able to use their services
    - example: Google AI studio

- train
  - unsloth
    - google colab
      - i could have used my own laptop, cause it's a 1b model
      - but installing anything advanced on python is a pain
  - google ai lab

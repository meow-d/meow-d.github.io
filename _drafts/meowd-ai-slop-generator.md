I kept my promise. I've created the cringe generator.

here's link of some AI slop it generated.

TODO cohost link, slop link

- used
  - download data from cohost-dl
    - posts.json file
  - python
    - parse json
      - remove shares
        - ["astmap"][""] = []
      - only included post text
        - "headline" and "rawtextcontent(?)"
    - convert to csv

- multiple ways you can format the dataset
  - title as input, post as output
  - "write a cohost post" as input, title + post as output
  - no input, just title + post as output
    - you're essentially not fine tuning for a specific purpose, but a general slop generator that you can't even converse with

- models
  - i chose a 1b one cause... i'm a pussy

- train
  - unsloth
    - google colab
      - i could have used my own laptop, cause it's a 1b model
      - but installing anything advanced on python is a pain
  - google ai lab

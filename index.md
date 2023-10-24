---
layout: default
---

I am a Senior Researcher at Microsoft Research Redmond in the <a href="https://www.microsoft.com/en-us/research/group/augmented-learning-and-reasoning/" target="_blank">Augmented Learning and Reasoning</a> group. I focus on evaluating and improving large language model-based conversational systems. I graduated from the University of Michigan in May 2022 with a PhD in computer science working with <a href="http://danaikoutra.com" target="_blank">Danai Koutra</a> on text-augmented graph learning. 

See <a href="https://scholar.google.com/citations?hl=en&user=bIWFjekAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a> for an up-to-date publications list.

__Contact__: tarasafavi \[at\] microsoft.com

## Recent news

{% for news in site.data.news limit:7 %}
- __{{ news.date }}__: {{ news.description }} {% endfor %}

## Misc (updated periodically)

  - My <a href="/nsf-grfp.html">advice on applying for the NSF GRFP</a>, last updated in 2020
  - All-time favorite books/audiobooks {% for book in site.data.reading %}
    - <a href="{{ book.link }}" target="_blank">{{ book.title }}</a> by {{ book.author }}  {% if book.notes %} - <em>{{ book.notes }}</em> {% endif %} {% endfor %}

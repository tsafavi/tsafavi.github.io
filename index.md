---
layout: default
---

I am a deep learning engineer at NVIDIA, working on inference co-design for frontier models and agents. Previously, I was a researcher at Microsoft Research + M365 Copilot working on pre-agentic agentic workflows, including external memory and retrieval, LLM judge and verification, and looping of AI models. I graduated from the University of Michigan in May 2022 with a PhD in machine learning.

See <a href="https://scholar.google.com/citations?hl=en&user=bIWFjekAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a> for an up-to-date publications list.

__Contact__: tsafavi \[at\] nvidia.com

## Recent news

{% for news in site.data.news limit:7 %}
- __{{ news.date }}__: {{ news.description }} {% endfor %}

## Misc (updated periodically)

  - My <a href="/nsf-grfp.html">advice on applying for the NSF GRFP</a>, last updated in 2020
  - All-time favorite books/audiobooks {% for book in site.data.reading %}
    - <a href="{{ book.link }}" target="_blank">{{ book.title }}</a> by {{ book.author }}  {% if book.notes %} - <em>{{ book.notes }}</em> {% endif %} {% endfor %}

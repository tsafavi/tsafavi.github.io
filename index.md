---
layout: default
---

Hi! 
I'm Tara, a PhD candidate at the University of Michigan working with <a href="http://danaikoutra.com" target="_blank">Danai Koutra</a>.
My research focuses on relational learning and reasoning, knowledge representations, and graph-based machine learning.
I'm currently supported by an NSF Graduate Research Fellowship and a Google Women Techmakers scholarship.

Outside of work, I like to play and listen to music, stay healthy, and generally chill out.

## Recent news

{% for news in site.data.news limit:7 %}
- __{{ news.date }}__: {{ news.description }} {% endfor %}

## Selected publications

Also see <a href="https://scholar.google.com/citations?hl=en&user=bIWFjekAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a>, my <a href="cv.pdf">CV</a>.

{% for publication in site.data.publications %}
-  __{{ publication.title }}__ <br/> {{ publication.authors }} <br/> {{ publication.venue }} {{ publication.date }}
{% for link in publication.links %} {% if link.pdf %} <a href="{{ link.pdf }}" target="_blank">[PDF]</a>{% endif %}{% if link.slides %}  <a href="{{ link.slides }}" target="_blank">[slides]</a>{% endif %}{% if link.code %} <a href="{{ link.code }}" target="_blank">[GitHub]</a>{% endif %}{% if link.data %} <a href="{{ link.data }}" target="_blank">[GitHub]</a>{% endif %}{% if link.blog %} <a href="{{ link.blog }}" target="_blank">[blog
  post]</a>{% endif %}{% endfor %}{% if publication.highlight %}<br/> <span class="red">{{ publication.highlight }}</span>{% endif %}{% if publication.notes %}<br/> _{{ publication.notes }}_{% endif %} 

  {% endfor %}

## Misc

  - My <a href="/nsf-grfp.html">advice on applying for the NSF GRFP</a> (updated periodically)
  - Books I enjoyed reading recently: {% for book in site.data.reading %}
    - <a href="{{ book.link }}" target="_blank">{{ book.title }}</a> by {{ book.author }}  {% if book.notes %} - {{ book.notes }} {% endif %} {% endfor %}

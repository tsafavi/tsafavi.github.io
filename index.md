---
layout: default
---

Hi! 
I'm Tara, a final-year PhD candidate at the University of Michigan working with <a href="http://danaikoutra.com" target="_blank">Danai Koutra</a>.
My research focuses on machine learning over graphs + text and relational knowledge representation. 
I'm currently supported by an NSF Graduate Research Fellowship and a Google Women Techmakers scholarship.

<span class="red">In June 2022, I will join Microsoft Research Redmond as a research scientist.</span>

## Recent news

{% for news in site.data.news limit:7 %}
- __{{ news.date }}__: {{ news.description }} {% endfor %}

## Selected publications

Also see <a href="https://scholar.google.com/citations?hl=en&user=bIWFjekAAAAJ&view_op=list_works&sortby=pubdate" target="_blank">Google Scholar</a>, my <a href="cv.pdf">CV</a>.

{% for publication in site.data.publications %}
-  __{{ publication.title }}__ <br/> {{ publication.authors }} <br/> {{ publication.venue }} {{ publication.date }}
{% for link in publication.links %} {% if link.pdf %} <a href="{{ link.pdf }}" target="_blank">[PDF]</a>{% else %} [PDF coming soon] {% endif %}{% if link.slides %}  <a href="{{ link.slides }}" target="_blank">[slides]</a>{% endif %}{% if link.code %} <a href="{{ link.code }}" target="_blank">[GitHub]</a>{% endif %}{% if link.data %} <a href="{{ link.data }}" target="_blank">[GitHub]</a>{% endif %}{% if link.blog %} <a href="{{ link.blog }}" target="_blank">[blog
  post]</a>{% endif %}{% endfor %}{% if publication.highlight %}<br/> <span class="red">{{ publication.highlight }}</span>{% endif %}{% if publication.notes %}<br/> _{{ publication.notes }}_{% endif %} 

  {% endfor %}

## Misc

  - My <a href="/nsf-grfp.html">advice on applying for the NSF GRFP</a> (updated periodically)
  - Books I enjoyed recently: {% for book in site.data.reading %}
    - <a href="{{ book.link }}" target="_blank">{{ book.title }}</a> by {{ book.author }}  {% if book.notes %} - <em>{{ book.notes }}</em> {% endif %} {% endfor %}

---
layout: default
---

Hi! 
I'm Tara, a final-year PhD candidate at the University of Michigan working with <a href="http://danaikoutra.com" target="_blank">Danai Koutra</a>.
My research focuses on multimodal language + graph learning for problems in machine knowledge representation.
I'm currently supported by an NSF Graduate Research Fellowship and a Google Women Techmakers scholarship.


<span class="red">⭐ I'm on the job market for industry NLP + ML research scientist and research engineer positions starting 2022!! ⭐</span> Please find my <a href="cv.pdf" target="_blank">full-length academic CV</a> and <a href="resume.pdf" target="_blank">shorter technical resume</a>, and reach out if you think I'd be a good fit! 

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

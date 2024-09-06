---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 1
pubs:
  - author: "Author1, Author2"
    title: ""
    month: "April"
    year: "2022"
    booktitle: "title"
    url: "something.pdf"

  - author: ""
    title: ""
    month: "April"
    year: "2022"
    booktitle: ""
    url: ""


---

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

## patents

See [Google Patent Search results](https://patents.google.com/?inventor=Muntasim+Ul+Haque,-Lango&num=100&sort=old).

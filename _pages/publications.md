---
layout: archive
title: "Publications"
permalink: /publications/
---

{% assign sorted = site.publications | sort: "date" | reverse %}

{%- for pub in sorted -%}

  <div class="content-block">

    {{ pub.authors }}
    {% if pub.in-prep %}
    (in prep).
    {% elsif pub.submitted %}
    (submitted).
    {% elsif pub.under-review %}
    (under review).
    {% else %}
    ({{ pub.date | date: "%Y" }}
    {%- if pub.in-press -%}, in press {%- endif -%}).
    {% endif %}

    {% if pub.doi %} <a href="{{ pub.doi }}" target="_blank"> {% endif %} {{ pub.title }}{%- if pub.doi -%} </a> {%- endif -%}.

    {% if pub.editor %}
    In {{ pub.editor }} (Ed.),
    {% endif %}

    {%- if pub.journal -%}
    <i> {{ pub.journal }}</i>
    {%- if pub.volume -%}, {{ pub.volume }}
    {%- if pub.issue -%}({{ pub.issue }}){%- endif -%}
    {%- endif -%}
    {%- if pub.pages -%}, {{ pub.pages }}
    {%- endif -%}.
    {%- endif -%}

    {% if pub.publisher %}
    {{ pub.publisher }}.
    {% endif %}

    {% if pub.ref-1-name %} [<a href="{{ pub.ref-1-link }}" target="_blank">{{ pub.ref-1-name }}</a>

      {%- if pub.ref-2-name -%}, <a href="{{ pub.ref-2-link }}" target="_blank">{{ pub.ref-2-name }}</a>

        {%- if pub.ref-3-name -%}, <a href="{{ pub.ref-3-link }}" target="_blank">{{ pub.ref-3-name }}</a>

          {%- if pub.ref-4-name -%}, <a href="{{ pub.ref-4-link }}" target="_blank">{{ pub.ref-4-name }}</a>]

          {%- else -%}
          ]

          {%- endif -%}

        {%- else -%}
        ]

        {%- endif -%}
        
      {%- else -%}
      ]

      {%- endif -%}

    {% endif %}

    <div class="content-note">
      {{ pub.content }}
    </div>

  </div>

{% endfor %}

You can also find my articles on <u><a href="https://scholar.google.com/citations?user=mM5ehUQAAAAJ&hl=en">my Google Scholar profile</a>.</u>
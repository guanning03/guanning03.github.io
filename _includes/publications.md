<h2 id="publications" style="margin: 2px 0px -15px;">Publications</h2>

<div class="publications">
<p class="pub-legend">* denotes equal contribution.</p>
<ol class="bibliography">

{% for link in site.data.publications.main %}
{% assign project = link.page | default: link.code | default: link.pdf %}

<li>
<div class="pub-row">
  {% if link.image %}
  <div class="abbr">
    <img src="{{ link.image }}" class="teaser" alt="{{ link.title | escape }}" loading="lazy">
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short }}</abbr>
    {% endif %}
  </div>
  {% elsif link.conference_short %}
  <div class="venue">
    <abbr class="badge">{{ link.conference_short }}</abbr>
  </div>
  {% endif %}
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ link.pdf }}">{{ link.title }}</a></div>
      <div class="author">{{ link.authors }}</div>
    <div class="links" style="margin: 4px 0;">
      <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Paper</a>
      <a href="{{ project }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
    </div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
      {% if link.notes %}
      <div class="notes"><strong><i style="color:#e74d3c">{{ link.notes }}</i></strong></div>
      {% endif %}
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>

<h2 id="projects" style="margin: 2px 0px -15px;">Projects</h2>

<div class="projects">
  <ol class="bibliography">

    {% for project in site.data.projects.main %}
    <li>
      <div class="pub-row">
        <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
          {% if project.image %}
          <img src="{{ project.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
          {% endif %}
        </div>
        <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
          <div class="title"><a href="{{ project.pdf }}">{{ project.title }}</a></div>
          <div class="author">{{ project.authors }}</div>
          <div class="periodical"><em>{{ project.notes }}</em></div>
          <div class="links">
            {% if project.pdf %}
            <a href="{{ project.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; border: 1px solid #ccc; padding: 2px 8px; border-radius: 3px;">PDF</a>
            {% endif %}
            {% if project.code %}
            <a href="{{ project.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px; border: 1px solid #ccc; padding: 2px 8px; border-radius: 3px;">Code</a>
            {% endif %}
          </div>
        </div>
      </div>
    </li>
    <br>
    {% endfor %}

  </ol>
</div>
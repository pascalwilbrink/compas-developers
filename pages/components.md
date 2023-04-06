---
layout: default
---

# Components

<div class="components">
    {% for component in site.components %}
        <div class="components_component">
            <div class="card">
                <div class="card__header">
                    {{ component.name }}
                </div>
                <div class="card__content">
                    <a href="{{ component.url | relative_url }}">
                        Card content
                    </a>
                </div>
                <div class="card__actions">
                    {% if component.urls %}
                        <div class="component__logos">
                            {% if component.urls.storybook %}
                                <a href="{{ component.urls.storybook }}" target="_blank">
                                    <img src="{{ site.baseurl }}/assets/images/storybook.png" class="component__logo" />
                                </a>
                            {% endif %}
                            {% if component.urls.github %}
                                <a href="{{ component.urls.github }}" target="_blank">
                                    <img src="{{ site.baseurl }}/assets/images/github.png" class="component__logo" />
                                </a>
                            {% endif %}
                            {% if component.urls.npm  %}
                                <a href="{{ component.urls.npm }}" target="_blank">
                                    <img src="{{ site.baseurl }}/assets/images/npm.png" class="component__logo" />
                                </a>
                            {% endif %}
                        </div>
                    {% endif %}
                </div>
            </div>
        </div>
    {% endfor %}
</div>

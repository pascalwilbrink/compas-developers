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
                    <div class="component__logos">
                        {% if component.storybook %}
                            <a href="{{ component.storybook }}" target="_blank">
                                <img src="{{ site.url }}/assets/images/storybook.png" class="component__logo" />
                            </a>
                        {% endif %}
                        {% if component.github %}
                            <a href="{{ component.github }}" target="_blank">
                                <img src="{{ site.url }}/assets/images/github.png" class="component__logo" />
                            </a>
                        {% endif %}
                        {% if component.npm  %}
                            <a href="{{ component.npm }}" target="_blank">
                                <img src="{{ site.url }}/assets/images/npm.png" class="component__logo" />
                            </a>
                        {% endif %}
                    </div>
                </div>
            </div>
        </div>
    {% endfor %}
</div>

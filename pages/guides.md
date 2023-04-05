---
layout: default
---

# Guides

<div class="guides">
    {% for guide in site.guides %}
        <div class="guides__guide">
            <div class="card">
                <div class="card__header">
                    <a href="{{ guide.url | relative_url }}">{{ guide.name }}</a>
                    {{ guide.summary }}
                </div>
            </div>
        </div>
    {% endfor %}
</div>



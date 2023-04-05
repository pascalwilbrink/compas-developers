---
layout: default
---

# Plugins

<div class="plugins">
    {% for plugin in site.compas_plugins %}
        <div class="plugins__plugin">
            <div class="card">
                <div class="card__header">
                    {{ plugin.name }}
                </div>
            </div>
        </div>
    {% endfor %}
</div>



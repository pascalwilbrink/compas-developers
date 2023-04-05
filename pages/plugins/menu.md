---
layout: default
---

# Menu Plugins

<div class="plugins">
    {% assign plugins = site.compas_plugins | where: "plugin_type", "menu" %}
    {% for plugin in plugins %}
        <div class="plugins__plugin">
            <div class="card">
                <div class="card__header">
                    {{ plugin.name }}
                </div>
            </div>
        </div>
    {% endfor %}
</div>



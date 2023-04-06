---
layout: default
---

<aside>
    <div class="card">
        <div class="card__content">
            <ul class="list">
                <li class="list__item">
                    <a href="{{ site.baseurl }}/pages/plugins">
                        All
                    </a>
                </li>
                <li class="list__item">
                    <a href="{{ site.baseurl }}/pages/plugins/menu">
                        Menu
                    </a>
                </li>
                <li class="list__item">
                    <a href="{{ site.baseurl }}/pages/plugins/editor">
                        Editor
                    </a>
                </li>
            </ul>
        </div>
    </div>
</aside>
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



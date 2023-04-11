---
name: Create Plugin
layout: guide
summary: | 
    In this guide, we will show you how you can easily create a plugin for CoMPAS OpenSCD.
toc: true
---

## Intro
In this guide, we will show you how you can easily create a plugin for CoMPAS OpenSCD.
\
In this example, we will make use of [lit-element](https://www.lit.dev){:target="_blank"} as a custom Webcomponent framework.
\
We will follow the standards from [Open-wc](https://open-wc.org){:target="_blank"}.


## Prerequisites
* [NodeJS](https://nodejs.org)
* [GitHub](https://www.github.com) account

## Install CLI Tool

To install the cli tool for the plugin, you can use the following command:

{% capture code %}
    {% highlight shell %}
        npm install @openscd/cli --global
    {% endhighlight %}
{% endcapture %}

{% include code.md code=code %}

\
With the CLI tool, we can setup a boilerplate for the plugin.

Use the following command to create the boilerplate:

{% capture code %}
    {% highlight shell %}
        oscd new plugin
    {% endhighlight %}
{% endcapture %}

{% include code.md code=code %}
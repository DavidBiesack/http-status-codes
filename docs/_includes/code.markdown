<!--
     this is an include so that the long Liquid template code does not
     exceed the markdownlint limit on line lengths, but still allowing
     `markdownlint` to lint the rest of `../index.md`.
     The template is all on one line to prevent injecting extra newlines
     (paragraphs) in the generated ../_site/index.html page
     which we end up with if we format this source more nicely with
     newlines
-->
{%- assign groupNum = 0 -%}
{% for page in site.pages %}{% if page.set %}{% if page.set > groupNum %}{% assign groupNum = page.set %}{% assign group = groupNum | append: "" %}<span class="group group{{group}}" title="{{ site.data.groups.descriptions[group] }}">{{ group }}&times;&times;</span> - <span title="{{ site.data.groups.descriptions[group] }}">{{ site.data.groups.titles[group] }}</span><br>{% endif %}<a class="status-code group{{group}}" href="./{{ page.code }}">{{ page.code }}</a> <a href="./{{ page.code }}">{{ page.title }}</a><br>{% endif %}{% endfor %}

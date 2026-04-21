---
layout: default
lang: zh
title: 首页
permalink: /zh/
---

<h1>BITBLOG 中文版</h1>
<p>关于 BITBOX 开发平台和 Bitcoin Cash 生态系统最新动态的博客。</p>
<p>了解更多 BITBOX 信息，请访问 <a href="https://www.bitbox.earth">bitbox.earth</a></p>

{% assign posts = site.posts | where: "lang", "zh" %}
{% for post in posts %}
  <h2>{{ post.title }}</h2>
  <p>{{ post.excerpt }}</p>
  <a href="{{ post.url }}">阅读更多...</a>
{% endfor %}

{% if posts.size == 0 %}
  <p><em>中文文章即将上线，敬请期待！</em></p>
{% endif %}

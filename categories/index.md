---
layout: page
title: 文章分类
permalink: /categories/
---

<div class="categories-list">
    <div class="category-section">
        <h2>德国生活</h2>
        <p>{{ site.category_settings.life.description }}</p>
        <ul>
            {% for post in site.categories['Life in Germany'] %}
            <li>
                <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </li>
            {% endfor %}
        </ul>
    </div>

    <div class="category-section">
        <h2>工作求职</h2>
        <p>{{ site.category_settings.work.description }}</p>
        <ul>
            {% for post in site.categories['Working in Germany'] %}
            <li>
                <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </li>
            {% endfor %}
        </ul>
    </div>

    <div class="category-section">
        <h2>学习德语</h2>
        <p>{{ site.category_settings.german.description }}</p>
        <ul>
            {% for post in site.categories['Learn German'] %}
            <li>
                <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
                <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
            </li>
            {% endfor %}
        </ul>
    </div>
</div> 
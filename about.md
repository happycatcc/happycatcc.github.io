---
layout: default
title: 关于我
permalink: /about/
---

<div class="about-page">
    <div class="about-header">
        <div class="avatar">
            <img src="{{ site.author.avatar | relative_url }}" alt="{{ site.author.name }}">
        </div>
        <h1>你好呀 👋</h1>
        <p class="intro">我是CC猫，一只从2014年就漂洋过海来到德国的程序猫</p>
    </div>

    <div class="timeline">
        <div class="timeline-item">
            <div class="time">2014</div>
            <div class="content">
                <h3>🛫 来到德国</h3>
                <p>带着对未知的期待，开始了在德国的留学生活</p>
            </div>
        </div>

        <div class="timeline-item">
            <div class="time">2014-2017</div>
            <div class="content">
                <h3>📚 求学时光</h3>
                <p>在德国攻读硕士学位，经历了许多第一次：第一次用德语点餐、第一次独自旅行、第一次在异国过年...</p>
            </div>
        </div>

        <div class="timeline-item">
            <div class="time">2017至今</div>
            <div class="content">
                <h3>💻 工作生活</h3>
                <p>毕业后选择留在德国工作，成为一名程序员。在这里扎根，让异国他乡变成了第二个家。</p>
            </div>
        </div>
    </div>

    <div class="about-section">
        <h2>为什么写这个博客</h2>
        <p>十年前，我也和很多人一样，怀着憧憬来到德国。这些年经历了语言关卡、文化差异、找工作等各种挑战，也收获了很多难忘的经历和成长。</p>
        <p>建立这个博客是为了：</p>
        <ul>
            <li>📝 记录在德国的生活点滴</li>
            <li>💼 分享程序员在德国的工作经验</li>
            <li>🗣️ 交流学习德语的心得</li>
            <li>🤝 帮助想来德国发展的朋友</li>
        </ul>
    </div>

    <div class="about-section">
        <h2>博客内容</h2>
        <div class="content-cards">
            <div class="card">
                <h3>🏠 德国生活</h3>
                <p>从柴米油盐到文化差异，记录最真实的德国生活。</p>
            </div>
            <div class="card">
                <h3>💼 工作经验</h3>
                <p>分享程序猫在德国工作的所见所闻，以及求职经验。</p>
            </div>
            <div class="card">
                <h3>📚 德语学习</h3>
                <p>记录学习德语的过程，分享实用的学习资源。</p>
            </div>
        </div>
    </div>

    <div class="about-section contact">
        <h2>联系我</h2>
        <p>如果你也对德国生活感兴趣，欢迎通过以下方式找我聊天：</p>
        <div class="contact-methods">
            <a href="mailto:{{ site.author.email }}" class="contact-item">
                <i class="far fa-envelope"></i>
                <span>Email</span>
            </a>
            {% for social in site.social %}
            <a href="{{ social.url }}" class="contact-item" target="_blank">
                {% if social.title == "xiaohongshu" %}
                <i class="fas fa-book" style="color: #ff2442;"></i>
                {% elsif social.title == "x-twitter" %}
                <i class="fa-brands fa-x-twitter"></i>
                {% else %}
                <i class="fab fa-{{ social.title }}"></i>
                {% endif %}
                <span>{{ social.title | capitalize }}</span>
            </a>
            {% endfor %}
        </div>
    </div>
</div>

---

> "人生就是一场经历，重要的不是目的地，而是沿途的风景和故事。" 
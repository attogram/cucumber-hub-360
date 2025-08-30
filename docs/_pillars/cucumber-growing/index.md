---
layout: default
title: Cucumber Growing Techniques
excerpt: "Your complete guide to growing cucumbers at home. From choosing the right variety and preparing your soil to pest control and harvesting, we have you covered."
image: /assets/img/card-recipe-01.png
---

<div class="container py-4">
    <header class="text-center">
        <h1>{{ page.title }}</h1>
        <p class="lead">{{ page.excerpt }}</p>
    </header>

    <div class="grid py-4">
        {% assign pillar_posts = site['cucumber-growing'] | sort: 'date' | reverse %}
        {% for post in pillar_posts %}
            {% if post.url != page.url %}
                <div class="col-span-12 md:col-span-4">
                    {% include card.html post=post %}
                </div>
            {% endif %}
        {% endfor %}
    </div>

    <hr>

    <aside class="text-center py-4">
        <h3>Related Pillars</h3>
        <p>
            Once you've grown them, find a use for them in <a href="#">All-Cucumber Recipes</a> or learn about <a href="#">Smart Cucumber Farming</a> for larger scale operations.
        </p>
    </aside>

</div>

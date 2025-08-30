---
layout: default
title: Cucumber Skincare & Detox Programs
excerpt: "Discover the natural power of cucumbers for your skin and body. Explore our DIY beauty recipes, detox water plans, and expert advice for a refreshed and glowing you."
image: /assets/img/card-recipe-02.png
---

<div class="container py-4">
    <header class="text-center">
        <h1>{{ page.title }}</h1>
        <p class="lead">{{ page.excerpt }}</p>
    </header>

    <div class="grid py-4">
        {% comment %}
        This will loop through all documents in this collection and display them.
        {% endcomment %}
        {% assign pillar_posts = site['cucumber-skincare-detox'] | sort: 'date' | reverse %}
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
            Learn about the science in our <a href="#">Scientific Research</a> pillar, or find healthy recipes in <a href="#">All-Cucumber Recipes</a>.
        </p>
    </aside>

</div>

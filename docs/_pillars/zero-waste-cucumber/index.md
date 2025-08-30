---
layout: default
title: Zero-Waste Cucumber Guides
excerpt: "Embrace sustainability with our zero-waste cucumber guides. Learn how to use every part of the plant, from peels to seeds, with creative upcycling ideas, footprint calculators, and composting tips."
image: /assets/img/card-recipe-03.png
---

<div class="container py-4">
    <header class="text-center">
        <h1>{{ page.title }}</h1>
        <p class="lead">{{ page.excerpt }}</p>
    </header>

    <div class="grid py-4">
        {% assign pillar_posts = site['zero-waste-cucumber'] | sort: 'date' | reverse %}
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
            Learn about the bigger picture in our <a href="#">Environmental Impact</a> pillar, or get your hands dirty with our <a href="#">Cucumber Growing</a> guides.
        </p>
    </aside>

</div>

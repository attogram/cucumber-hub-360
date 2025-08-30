---
layout: default
title: All-Cucumber Recipes
excerpt: "Explore a world of culinary delight with our extensive collection of recipes where cucumber is the star. From refreshing salads and chilled soups to innovative cocktails and savory pickles, find your next favorite dish here."
image: /assets/img/card-recipe-01.png
---

<div class="container py-4">
    <header class="text-center">
        <h1>{{ page.title }}</h1>
        <p class="lead">{{ page.excerpt }}</p>
    </header>

    <div class="grid py-4">
        {% comment %}
        This will loop through all documents in the 'all-cucumber-recipes' collection
        and display them using the card partial.
        {% endcomment %}
        {% assign pillar_posts = site['all-cucumber-recipes'] | sort: 'date' | reverse %}
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
            After you've found a recipe, learn about <a href="#">Cucumber Beverages & Cocktails</a> or explore <a href="#">Special-Diet Recipes</a>.
        </p>
    </aside>

</div>

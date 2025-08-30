---
layout: default
title: Home
---

<style>
.hero-section {
    background-size: cover;
    background-position: center;
    padding: 6rem 1.5rem;
    color: white;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 400px;
    border-bottom: 4px solid var(--cuke-green-500);
}
.hero-content {
    max-width: 800px;
}
.hero-content h1 {
    color: white;
    font-size: clamp(2rem, 5vw, 3.5rem);
    margin-bottom: 0.5rem;
}
.tagline {
    font-size: clamp(1.1rem, 2vw, 1.5rem);
    font-weight: 400;
}
</style>

<header class="hero-section" style="background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('{{ '/assets/img/hero-cucumber.png' | relative_url }}');">
    <div class="hero-content text-center">
        <h1>Cucumber Hub 360°</h1>
        <p class="tagline">{{ site.description }}</p>
        <a href="#pillars" class="btn">Explore the Hub</a>
    </div>
</header>

<div id="pillars" class="container py-4">
    <h2 class="text-center" style="margin-bottom: 2rem;">Explore Our Content Pillars</h2>
    <div class="grid">
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">All-Cucumber Recipes</a></h3>
                    <p>From refreshing salads to surprising main courses, discover recipes where cucumber is the star.</p>
                </div>
            </div>
        </div>
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">Cucumber Skincare</a></h3>
                    <p>Unlock the secrets of cucumber for your skin with our DIY beauty formulas and detox programs.</p>
                </div>
            </div>
        </div>
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">Cucumber Growing</a></h3>
                    <p>Everything you need to know, from planting calendars to pest control for a bountiful harvest.</p>
                </div>
            </div>
        </div>
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">Scientific Research</a></h3>
                    <p>We summarize peer-reviewed studies on cucumber nutrition and health benefits.</p>
                </div>
            </div>
        </div>
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">Zero-Waste Cucumber</a></h3>
                    <p>Learn creative upcycling ideas and use our calculators to measure your environmental footprint.</p>
                </div>
            </div>
        </div>
        <div class="col-span-12 md:col-span-4">
            <div class="card">
                <div class="card__content">
                    <h3 class="card__title"><a href="#">And many more...</a></h3>
                    <p>Explore all 37 pillars covering history, art, market data, food safety, and more!</p>
                </div>
            </div>
        </div>
    </div>
</div>

---
layout: default
title: Home
description: Welcome to the Glen Rock Historical and Preservation Society - Preserving and sharing the history of Glen Rock, New Jersey
---

<div class="relative">
    <!-- Hero section with background image -->
    <div class="h-[60vh] bg-cover bg-center" style="background-image: url('/assets/images/glen-rock-hero.jpg');">
        <div class="absolute inset-0 bg-black bg-opacity-50"></div>
        <div class="relative h-full flex items-center justify-center text-center text-white px-4">
            <div>
                <h1 class="text-4xl md:text-6xl font-bold mb-4">Glen Rock Historical & Preservation Society</h1>
                <p class="text-xl md:text-2xl mb-8">Preserving Our Past, Enriching Our Future</p>
                <a href="/about" class="bg-grhps-accent hover:bg-grhps-primary text-white font-bold py-3 px-8 rounded-lg transition duration-300">
                    Learn More
                </a>
            </div>
        </div>
    </div>
</div>

<div class="py-16">
    <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Museum Information -->
            <div class="bg-white rounded-lg shadow-lg p-6">
                <h2 class="text-2xl font-bold text-grhps-primary mb-4">Visit Our Museum</h2>
                <p class="mb-4">The Museum at the Station is open on the last Sunday of each month from 1:00 PM to 3:00 PM. Discover Glen Rock's rich history through our rotating exhibits and permanent collections.</p>
                <a href="/about#museum" class="text-grhps-primary hover:text-grhps-accent font-semibold">Plan your visit →</a>
            </div>

            <!-- Upcoming Events -->
            <div class="bg-white rounded-lg shadow-lg p-6">
                <h2 class="text-2xl font-bold text-grhps-primary mb-4">Upcoming Events</h2>
                <ul class="space-y-4">
                    {% for event in site.events limit:3 %}
                    <li>
                        <span class="block text-sm text-gray-500">{{ event.date | date: "%B %d, %Y" }}</span>
                        <a href="{{ event.url }}" class="font-medium hover:text-grhps-accent">{{ event.title }}</a>
                    </li>
                    {% endfor %}
                </ul>
                <a href="/events" class="mt-4 inline-block text-grhps-primary hover:text-grhps-accent font-semibold">View all events →</a>
            </div>

            <!-- Get Involved -->
            <div class="bg-white rounded-lg shadow-lg p-6">
                <h2 class="text-2xl font-bold text-grhps-primary mb-4">Get Involved</h2>
                <p class="mb-4">Support our mission to preserve Glen Rock's history. Join as a member, volunteer, or make a donation to help maintain our collections and programs.</p>
                <a href="/donate" class="inline-block bg-grhps-primary hover:bg-grhps-accent text-white font-bold py-2 px-4 rounded transition duration-300">Support GRHPS</a>
            </div>
        </div>
    </div>
</div>

<div class="bg-gray-100 py-16">
    <div class="container mx-auto px-4">
        <h2 class="text-3xl font-bold text-center text-grhps-primary mb-12">Featured Resources</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
            <a href="/heritage-trail" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9 bg-gray-200">
                        <!-- Add image here -->
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Heritage Trail</h3>
                        <p class="text-sm text-gray-600">Explore Glen Rock's historic sites</p>
                    </div>
                </div>
            </a>
            
            <a href="/gallery" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9 bg-gray-200">
                        <!-- Add image here -->
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Photo Gallery</h3>
                        <p class="text-sm text-gray-600">Historical images of Glen Rock</p>
                    </div>
                </div>
            </a>
            
            <a href="/road2liberty" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9 bg-gray-200">
                        <!-- Add image here -->
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Road2Liberty</h3>
                        <p class="text-sm text-gray-600">Glen Rock's role in history</p>
                    </div>
                </div>
            </a>
            
            <a href="/veteran-banners" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9 bg-gray-200">
                        <!-- Add image here -->
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Veteran Banners</h3>
                        <p class="text-sm text-gray-600">Honoring our veterans</p>
                    </div>
                </div>
            </a>
        </div>
    </div>
</div>

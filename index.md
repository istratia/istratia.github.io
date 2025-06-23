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
        <!-- Museum Video Section -->
        <div class="mb-16">
            <h2 class="text-3xl font-bold text-grhps-primary mb-8 text-center">Welcome to The Museum at the Station</h2>
            <div class="max-w-4xl mx-auto">
                <div class="aspect-w-16 aspect-h-9 rounded-lg overflow-hidden shadow-xl">
                    <video controls class="w-full h-full object-cover">
                        <source src="https://video.wixstatic.com/video/ed30b6_5e594ec5d01d4194994869465e380d71/720p/mp4/file.mp4" type="video/mp4">
                        Your browser does not support the video tag.
                    </video>
                </div>
                <p class="mt-4 text-center text-gray-600">Take a virtual tour of our museum and discover Glen Rock's rich history.</p>
            </div>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- Museum Information -->
            <div class="bg-white rounded-lg shadow-lg p-6 hover:shadow-xl transition duration-300">
                <div class="flex items-center mb-4">
                    <svg class="h-8 w-8 text-grhps-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"/>
                    </svg>
                    <h2 class="text-2xl font-bold text-grhps-primary ml-3">Visit Our Museum</h2>
                </div>
                <p class="mb-4">The Museum at the Station is open on the last Sunday of each month from 1:00 PM to 3:00 PM. Discover Glen Rock's rich history through our rotating exhibits and permanent collections.</p>
                <a href="/about#museum" class="text-grhps-primary hover:text-grhps-accent font-semibold inline-flex items-center">
                    Plan your visit
                    <svg class="h-4 w-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/>
                    </svg>
                </a>
            </div>

            <!-- Upcoming Events -->
            <div class="bg-white rounded-lg shadow-lg p-6 hover:shadow-xl transition duration-300">
                <div class="flex items-center mb-4">
                    <svg class="h-8 w-8 text-grhps-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z"/>
                    </svg>
                    <h2 class="text-2xl font-bold text-grhps-primary ml-3">Upcoming Events</h2>
                </div>
                <ul class="space-y-4">
                    {% for event in site.events limit:3 %}
                    <li class="border-l-4 border-grhps-accent pl-4">
                        <span class="block text-sm text-gray-500">{{ event.date | date: "%B %d, %Y" }}</span>
                        <a href="{{ event.url }}" class="font-medium hover:text-grhps-accent">{{ event.title }}</a>
                    </li>
                    {% endfor %}
                </ul>
                <a href="/events" class="mt-6 inline-flex items-center text-grhps-primary hover:text-grhps-accent font-semibold">
                    View all events
                    <svg class="h-4 w-4 ml-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/>
                    </svg>
                </a>
            </div>

            <!-- Get Involved -->
            <div class="bg-white rounded-lg shadow-lg p-6 hover:shadow-xl transition duration-300">
                <div class="flex items-center mb-4">
                    <svg class="h-8 w-8 text-grhps-primary" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.828 14.828a4 4 0 01-5.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/>
                    </svg>
                    <h2 class="text-2xl font-bold text-grhps-primary ml-3">Get Involved</h2>
                </div>
                <p class="mb-6">Support our mission to preserve Glen Rock's history. Join as a member, volunteer, or make a donation to help maintain our collections and programs.</p>
                <div class="space-y-3">
                    <a href="/donate" class="block w-full bg-grhps-primary hover:bg-grhps-accent text-white text-center font-bold py-2 px-4 rounded-lg transition duration-300">
                        Become a Member
                    </a>
                    <a href="/contact#volunteer" class="block w-full border-2 border-grhps-primary text-grhps-primary hover:bg-grhps-primary hover:text-white text-center font-bold py-2 px-4 rounded-lg transition duration-300">
                        Volunteer With Us
                    </a>
                </div>
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
                    <div class="aspect-w-16 aspect-h-9">
                        <img src="/assets/images/heritage-trail.jpg" alt="Glen Rock Heritage Trail" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Heritage Trail</h3>
                        <p class="text-sm text-gray-600">Explore Glen Rock's historic sites</p>
                    </div>
                </div>
            </a>
            
            <a href="/gallery" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9">
                        <img src="/assets/images/photo-gallery.jpg" alt="Glen Rock Historical Photos" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Photo Gallery</h3>
                        <p class="text-sm text-gray-600">Historical images of Glen Rock</p>
                    </div>
                </div>
            </a>
            
            <a href="/road2liberty" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9">
                        <img src="/assets/images/road2liberty.jpg" alt="Glen Rock Road to Liberty" class="w-full h-full object-cover">
                    </div>
                    <div class="p-4">
                        <h3 class="font-bold group-hover:text-grhps-accent">Road2Liberty</h3>
                        <p class="text-sm text-gray-600">Glen Rock's role in history</p>
                    </div>
                </div>
            </a>
            
            <a href="/veteran-banners" class="group">
                <div class="bg-white rounded-lg shadow-lg overflow-hidden">
                    <div class="aspect-w-16 aspect-h-9">
                        <img src="/assets/images/veteran-banners.jpg" alt="Glen Rock Veteran Banners" class="w-full h-full object-cover">
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

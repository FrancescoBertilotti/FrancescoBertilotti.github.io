---
title: Making of this Website
categories: ["code"] 
tags: ["site", "portfolio", "hugo"]
params.dateFormat: ["13 November 2025"]
date: 2025-11-15
---  
## Introduction   
I built this place using Hugo, to share my projects, experiments, and whatever cool things I’m working on from music and sound design to electronics, coding, and random ideas.   
Before anything else: if you want to set up a website properly with Hugo and the Blowfish theme, I highly recommend reading the official documentation. It’s clear, complete, and way more detailed than anything I could cover here.
This post is just a short “behind the scenes” summary of how I built my setup — nothing too deep or technical, just the steps I followed and the things I found useful while putting the site together.   

## Official Page 
-[Hugo Offical Site](https://gohugo.io/)

-[Blowfish Offical Site](https://blowfish.page/)
   
## What I Needed   
Before starting this website, I had to be clear about what kind of place I wanted to build. I didn’t just want a random blog — I needed something that actually fit the way I work and the kind of projects I create. Basically, a space where I could drop everything I’m working on without overthinking it.   
Here’s what I knew I needed:   
- **A place to post all my projects** — music production stuff, sound design experiments, Max/MSP patches, Arduino/ESP32 builds, 3D printing ideas, home-lab setups, and whatever else I’m messing with.   
- ** easy to update** — I didn’t want a system that slows me down. Just write a post, save it, done.   
- **A clean structure** that keeps things organized without forcing me into a complicated workflow.   
- **A format I can version-control** — because being able to track changes (or undo my mistakes) is always a lifesaver.   
- **A tool that lets me customize things freely** if one day I decide to change the design, add sections, or tweak the layout.   
   
Hugo basically checked all these boxes right away   
   
## Why I Chose Hugo (and the Blowfish Theme)   
Once I figured out what kind of website I needed, choosing the tools became a lot easier. I wanted something fast, lightweight, and flexible — and **Hugo** instantly felt like the right fit. It doesn’t need a database, it builds pages in a second, and everything stays in plain files that I can edit whenever I want.   
For the theme, I went with **Blowfish**.   
I picked it mainly because the official documentation is super clear, well organized, and actually easy to follow — which is not always the case with themes. Everything is explained step-by-step, and it made the whole setup process feel smooth instead of frustrating. Plus, the theme looks clean, modern, and customizable enough for what I want to build here.   
So yeah, Hugo + Blowfish felt like the perfect combo to start this website without getting lost in a thousand settings.   
   
## How I Set Everything Up   
Setting up the website was actually way easier than I expected. Hugo is super fast to install, and once you get the basic folder structure, everything just clicks. Here’s how I set everything up step by step.   
### 1. Installing Hugo And Blowfish   
The first thing I did was install the **Extended version** of Hugo, since Blowfish needs it for SCSS and other advanced features.   
I installed it using Winget   
```
winget install Hugo.Hugo.Extended

```
Then I created a new Hugo site using:   
```
hugo new site my-website

```
This instantly gives you the folder structure   
```
my-site/
├── archetypes/
├── assets/
├── content/
├── data/
├── i18n/
├── layouts/
├── static/
├── themes/
└── hugo.toml
```
Next, I added the **Blowfish** theme using Git, following the official documentation   
```
git init
git submodule add -b main https://github.com/nunocoracao/blowfish.git themes/blowfish
```
One thing I liked about Blowfish from the start is how well the docs are written — everything is clear, organized, and easy to follow, which made customization super smooth.   
Once the theme was installed, I moved on to personalizing it. Blowfish comes with several built-in color schemes, and I decided to use the **Forest** palette   
### 2. Creating My First Post   
Once the website was running smoothly, it was time to actually add some content. In Hugo, all the pages and posts live inside the `content` folder, so that’s where everything needs to be placed. Since I wanted a clean structure for future articles, I created a new folder called `posts` inside `content` — this is where all my blog posts will go.   
For writing, I didn’t use a code editor at first. I already use [Anytype](https://anytype.io/) every day for notes and personal projects, so it felt natural to write the text for my first article there. After finishing the draft, I just exported the document as a Markdown file and dropped it directly into the `posts` folder I had created in the Hugo project   
   

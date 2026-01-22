---
title: Building with Antigravity
categories: ["Code", "AI"]
tags: ["google", "antigravity", "workflow", "hugo"]
params.dateFormat: ["22 January 2026"]
date: 2026-01-22
---

### A New Workflow
You might have noticed some changes around here efficiently. I recently updated this website, adding a custom SoundCloud widget to my music posts and implementing full multi-language support (Italian and English). But I didn't do it alone—or rather, I didn't do it the "traditional" way.

For these updates, I used **Antigravity**, an advanced agentic coding assistant from Google.

### Coding with an Agent
Unlike standard code completion tools, working with Antigravity feels more like pair programming with a proactive engineer. instead of just asking "how do I center a div", I gave it high-level goals:
*   "Add a SoundCloud widget to the top of the article."
*   "Make the widget look like it belongs to the site's theme."
*   "Translate the entire site into Italian."

### The Process
The most impressive part was watching it handle the complexity of the multi-language setup. It didn't just translate the text; it understood the structure of Hugo. It created the configuration files, set up the menu definitions for the new language, and even realized (after a quick debug) that it needed to create specific `_index.md` files for the section to render correctly in Italian.

It also handled the aesthetics. When I asked to integrate the SoundCloud player, it didn't just paste the iframe. It researched the site's "Forest" theme, found the primary color variable in the CSS, and customized the widget's color scheme to match perfectly, wrapping it in a responsive container.

### The Future of Building
This experience has shifted how I view personal projects. It removes the friction between having an idea ("I want this site in Italian") and the execution. It allows me to focus on the *what* and *why*, while the agent handles the heavy lifting of the *how*.

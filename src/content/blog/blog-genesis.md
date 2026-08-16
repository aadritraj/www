---
title: "Blog Genesis and What I Learned"
description: "On the creation of the perfect blog"
pubDate: "Aug 16 2026"
---

This post counts as the first canonical blog post here. This page documents
the decisions I made and why, as this has been quite a change of pace
for me. The purpose of this blog is to serve as a space for me to express my thoughts and
feelings about whatever I feel like is worth noting, which will be mostly covering tech.

# The Glorified Wall of Text

A blog is simply a glorified wall of text, just like a book, except polished, personalised and
far more likely to have pretty pictures. However, every person has a different opinion on how interactive
their wall of text should be for the reader in an era of flashy maximalist sites.

The main architecture powering this site comes down to one thing: that there is very little need for reactivity on a blog. 

# The entire stack --- Astro

This website is built entirely with Astro and Markdown. While Astro supports UI components from React, Vue, Svelte
and more, this site uses only its native components.

Here are some things I learned while creating this site.

## Astro compared to everything else

As my knowledge of frontend design is strictly limited to React with TanStack Router and Svelte with SvelteKit,
I'll be drawing comparisons with both of them.

The main difference with Astro is its take on shipping JavaScript. While React and Svelte focus on making reactivity fun,
**Astro focuses on making HTML fun**. Writing Astro feels like a simplified approach to 
writing HTML templates, as the end result of an Astro component is always basic HTML, unless...

Switching from writing static React to Astro has little friction -- once you're accustomed to the Astro component syntax,
it comes pretty naturally.

## Islands

A client island in Astro, as Astro's docs describe it,
**is an interactive widget floating in a sea of otherwise static, lightweight, server-rendered HTML**.
While this website makes no use of this feature, it's still worth noting.

This approach draws parallels with the Next.js Server Rendering model in my opinion. Much like Next.js, the server renders
the HTML before being sent to the client. Where Astro differs is in hydration.

While Next hydrates **everything**, Astro only incrementally **enhances** the static page with the power of JavaScript.

# The Design

The design of this blog owes a lot to my time on Hacker News. The simple, barebones aesthetic was shaped by the blogs I found there, most of which were on AI -- as that's all the rage in tech nowadays.

The simple typography and the use of whitespace were inspired by others' blog posts. I have perfected
neither, and probably never will. However, I have struck a pretty decent balance between the two to make 
for a pleasant reading experience. 

# Conclusion

Overall, while I could have simply stayed in my comfort zone and created this site in SvelteKit, I am 
glad to have learned a new web technology, in a world where web technologies are a dime a dozen.

As a reward for either reading or skimming through this post, here are two nuggets of information:
- The real first post, used for testing Markdown rendering, can be found [here](/blog/test-post).
- The spinning star in the header was inspired by the promotion material for Ye's album BULLY.

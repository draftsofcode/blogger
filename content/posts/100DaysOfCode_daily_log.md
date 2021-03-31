---
title: "100DaysOfCode Daily Log"
date: 2021-03-29T23:15:10-04:00
draft: true
---

# 100 Days Of Code - Log

### Day 0: Monday, March 29, 2021

**Today's Progress:** Wrote blog post announcing [#100DaysOfCode](https://www.100daysofcode.com/rules/).

**Thoughts:** Getting Hugo set up was pretty straightforward. However, I ran into challenges hosting on Render.com and decided to switch over to Netlify. My biggest challenge on Render.com is that after a few commits, it stopped watching the github repository and wouldn't rebuild the site. So, I switched over to Netlify which has, so far, rebuilt the site on every commit. 

The other interesting thing is that there is no way to change an image's size in generic Markdown. So, I ended up using the [figure](https://gohugo.io/content-management/shortcodes/#figure) shortcode which made this possible.

One other thing is that I wasn't able to get Google Analytics working yet. But, will definitely figure it out. May just need to modify the theme that I have been using.

Getting going and keeping going will likely be challenging. I just hope to get a straightforward playable version of the game going.

### Day 1: Tuesday, March 30, 2021

**Today's Progress:** Added Google Analytics and Newsletter signup to the blog homepage

**Thoughts:** Originally, I installed the [Mainroad](https://themes.gohugo.io/mainroad/) theme as a git submodule. However, there were some changes that I needed to make which worked better if I just copied the theme and included it as a subdirectory in my theme folder. This added it to my repository so that all of my changes would be included. Below is a list of a few of the changes:

1. Google Analytics v4 -- the hugo default was not working properly. So, I added my own partial that included the [Google Analytics](https://analytics.google.com) tag. I modified the Mainroad theme to include the partial. There is likely a more Hugo way of doing it that could override default behavior.

2. [TinyLetter](https://tinyletter.com/) Newsletter form -- I wanted to include a newsletter to make it easier for people to keep up with my progress. TinyLetter provides email capture for free and it also handles unsubscribes. This is awesome. I created a widget and then included it in the right nav.

3. I modified the template so that just the logo and subtitle would be in the header. The default Mainroad theme would only show the subtitle if the main title was also available. Additionally, the logo was too small whenever the title and subtitle were enabled. So, I modified the template to show just the logo and the subtitle without a requirement for a main text-based title.
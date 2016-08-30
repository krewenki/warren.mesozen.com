---
layout: post
title: "Starting Over - (Re)Starting a blog in 2016"

---


I got laid off.  Just shy of 5 years of working on a project that never sold enough to even cover my salary, the
company decided it was time to trim some fat.  That happened almost 3 weeks ago.  Since then, i've been spending time
with my family, doing some house work, exercising, and just generally not touching a computer.  This morning, I had the
urge to pick up my laptop and work on something.  Anything.  I decided i'd focus on this blog again, for a short while.

The last post on this blog is from September 2013.  When that post was made, I was hosting on amazon S3, which has cost me about $0.33
per month, on average (I also store several GB of data there, so the number isn't solely this blog.).  While S3 is great, and
there is a jekyll gem/plugin that automatically builds and publishes to S3, I want to move things to a (DigitalOcean.com)[digitalocean.com]
droplet i've been running for the last year or two.

I need to make sure I have all the content from this site, preserve the url structure, upload it to my droplet, update DNS, install
an SSL certificate and try to get a valid HTTP 2 request in Chrome.  I'll keep a checklist running here while I do each task.

Make sure I have all the content
=====
This seems easy enough.  I've had a copy of this blog on github the whole time, so i've got what I need there.

Preserve URL Structure
=====
This should "just work", but when I try to build this locally with jekyll, I see no content.  I'll have to sort out the build errors in a 3 year old template.

Well, that was easy enough.  I was missing:
gems: [jekyll-paginate]
From my config.yml file.


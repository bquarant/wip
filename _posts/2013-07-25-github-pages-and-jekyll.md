---
layout: post
title:  "Github Pages and Jekyll"
date:   2013-07-25 16:27:26
categories: jekyll github-pages
---

I am a fan of Github Pages for web content publishing, and I have been using it to host my simple attempt at a [personal landing page][landing_page]. The biggest selling point for me is to be able to create and edit files and then fire off a quick ```git push``` in order to have my content published, and for just $7/month I think that it's one of the best services I pay for. 

Today I finally had a few spare hours that I could dedicate to getting this work in progress log off the ground, so I knew it was time to look into [Jekyll][jekyll_home], a powerful blog-aware static site generator.  I've known about of Jekyll for a long time, initially stemming from my brother's early involvement in the project and it's multitudinous successes. If you were to crawl through all of my commits on Github, you'll see that I have made some half-assed attempts at using Jekyll before, but I never got it to work before giving up. 

Progress Timeline: 
*  Generated new repository for the work (in) progress blog
*  Followed the basic steps to get Github Pages started...
*  Woohoo! <http://bquarant.github.io/wip/> now resolves to the right location
*  Struggled for a while after cloning new directory, couldn't get it to be 'blog-aware' 
*  Sucked it up and just ran ```jekyll new wip | cd wip | jekyll serve -w```
*  Cleaned up default scaffold code
*  Wrote 'Opening Salvo' blog entry, obligatory introductory stuff...
*  Learned some more Markdown formatting tricks
*  ```git push``` to gh-pages branch seemed like it worked fine...
*  CSS did not load on deployment, changed style sheet links in default.html to actual paths 
*  Links to blog post entries aren't working. They are currently going to <http://bquarant.github.io/jekyll/update/> instead of <http://bquarant.github.io/wip/jekyll/update/>
*  Solving local-side link issue...
*  Solving deployment-side link issue...
*  Started writing 'Github Pages and Jekyll' post


[landing_page]: http://bquarant.github.io/
[jekyll_home]: http://jekyllrb.com/
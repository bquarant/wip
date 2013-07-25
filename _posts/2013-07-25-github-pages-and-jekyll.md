---
layout: post
title:  "Github Pages and Jekyll"
date:   2013-07-25 16:27:26
categories: jekyll github-pages
---

**tl;dr -** 
Learning how to make Github Pages and Jekyll play nice together

I am a big fan of Github Pages for web content publishing, and I have been using it to host my simple attempt at a [personal landing page][landing_page]. The biggest selling point for me is to be able to create and edit files and then fire off a quick ```git push``` in order to have my content published on the internet, and for just $7/month I think that it's one of the best services I pay for. 

Today I finally had a few spare hours that I could dedicate to getting this work in progress log off the ground, so I knew it was time to figure out how to use [Jekyll][jekyll_home], a powerful blog-aware static site generator.  I've known about of Jekyll for a long time, initially stemming from my brother's early involvement in the project and it's multitudinous successes. If you were to crawl through all of my commits on Github, you'll see that I have made some half-assed attempts at using Jekyll before, but I never got it to work before giving up. 

After some initial difficulties originating from not really understanding the cloned Github Pages code, I wound up just pushing up a default fresh ```jekyll new``` and overwriting the Github Pages files. There was some trouble with making deployment and local paths resolve, but ultimately that wasn't too difficult. The new site now looks fine and the links function. To close the loop, I placed a new link on the landing page which points here.

**Progress Timeline** 
*  Generated new repository for the work (in) progress blog
*  Followed the basic steps to get Github Pages started...
*  Woohoo! <http://bquarant.github.io/wip/> now resolves to the right location
*  Struggled for a while after cloning new directory, [Github's help page][github_help_page] on the subject isn't all that helpful
*  Sucked it up and just ran ```jekyll new wip | cd wip | jekyll serve -w```
*  Cleaned up default scaffold code
*  Wrote 'Opening Salvo' blog entry, obligatory introductory stuff...
*  Learned some more Markdown formatting tricks
*  ```git push``` to gh-pages branch seemed like it worked fine...
*  CSS did not load on deployment, changed style sheet links in default.html to actual paths 
*  Links to blog post entries aren't working. They are currently going to <http://bquarant.github.io/jekyll/update/> instead of <http://bquarant.github.io/wip/jekyll/update/>
*  Turns out that this problem is due Jekyll configuration of the ```baseurl``` variable. Please refer to [Andrew Shell's][andrew_shell] [helpful post][fix_baseurl] on how to fix the ```baseurl``` configuration for Github Pages.
*  Solving deployment-side link ```baseurl``` issue: Add ```baseurl: /wip``` to ```_config.yml```
*  Solving local link ```baseurl``` issue: Duplicate and rename ```_config.yml``` to ```_config-local.yml```, Add ```baseurl: ``` to ```_config-local.yml```. Now you will need to run your local test server with ```jekyll serve -w --config _config-local.yml```, but paths are correct.
*  Added [gaug.es][gauges] support
*  Re-installed ImageMagick to have command line tools to manipulate images
*  Learned how to create markdown image links with Jekyll ``` ![]({{ site.baseurl }}/assets/file-name-of-image) ```

**Setting**
<div style="text-align:center;" markdown="1">
![]({{ site.baseurl }}/assets/hack-space-7-25-2013-2.jpg)
<br>
Boston College, O'Neill Library
</div>




[landing_page]: http://bquarant.github.io/
[jekyll_home]: http://jekyllrb.com/
[fix_baseurl]: https://github.com/andrewshell/baseurltest
[github_help_page]: https://help.github.com/articles/using-jekyll-with-pages
[andrew_shell]: http://blog.andrewshell.org/
[gauges]: http://gaug.es
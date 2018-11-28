---
layout: page
title: The assignment
permalink: /assignment/
---

In this assignment you are supposed to produce a web site that will be the front for your published assignments in this course and possibly in courses to come. The source code together with vagrant files etc. will be version controlled using git and pushed to the private YOURUSERNAME-examination-1-repo in 1dv022. However, the published site will be made public using your github-account and github-pages.

# Requirements

* Well designed - Well, what is well designed? We should at least see that you put some effort in your design and not just using the standard stuff

* All CSS should be generated from a CSS preprocessor

* Your site should have multiple pages, at least one where you present your self, your interest and so on and one blog page where you can present blog posts (more than one)

* Visitors should be able to comment on your posts (for instance you could use Disqus)

* Your site should have a robots.txt with your preferred configuration.

* Your site should have a humans.txt with your preferred configuration.

* You should use open graph for easy sharing on social media. You should at least use "title", "url", "type" and "image". You can check if it is working by sharing your site on for instance Facebook or Twitter.        

# Blog post

* Your blog page should have multiple posts (Swedish or English) and atleast one post where you reflects over the following:

* What do you think of pre-compiling your CSS?
    * Compare to regular CSS
    * Which techniques did you use?
    * Pros and cons?

* What do you think of static site generators?
    * What type of projects are they suitable for?

* What is robots.txt and how have you configure it for your site?

* What is humans.txt and how have you configure it for your site?

* How did you implements comments to blog posts

* What is Open Graph and how do you make use of it?

# Finishing up

When you feeling ready with your site it's time to publish it on GitHub Pages. GitHub Pages uses Jekyll by default so we can push the jekyll-files. OBS! The site you will publish is going to be public. Do the following.

1. Create a new empty public GitHub repositories and name it in the form <YOUR GITHUB USERNAME>.github.io

2. In your examination-repo add a new remote named "gh-pages" that points to your newly created github.io-repo run: git remote add gh-pages https://github.com/username/username.github.io

3. Check that you now have two remotes, one (origin) that points to your examination-repo and one (gh-pages) that points to your own github.io-repo run: git remote -v
4. To push your site in a correct way we need to push just our src-directory (the place where the jekyll-site is) and not the whole examination-repo (will include vagrant-files and other stuff) we have to use the "git subtree"-command run: git subtree push --prefix src gh-pages master --squash
5. Check your github.io-repo and use your browser to watch your site on: https://<YOUR GITHUB USERNAME>.github.io
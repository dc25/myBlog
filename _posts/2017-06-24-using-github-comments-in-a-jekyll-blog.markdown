---
layout: post
title: "Using Github comments in a Jekyll blog"
date: 2017-06-24 18:00:37 +0000
published: true
github_comments_issueid: "1"
tags:
---

### Background

A couple of months ago, Don Williamson demonstrated a clever technique for displaying Github issue comments on a static blog post.  He also provided a nice write up of the technique.

### Limitations

A limitation of the implementaion was that it was specific to the Hugo static site generator.  It turns out though that with minor changes, it can be integrated into a site based on Jekyll, another popular site generator.

### Jekyll

This blog is based on Jekyll and includes the changes needed to support use of Github comments.  This post has Github comments enabled so that the comments shown below are from a Github issue.  To add to those comments, click the "Post a comment on Github" link below.  This will take you to a Github page at which anyone can add a comment to the discussion that shows up on this page.  Github login is required to post a comment.

### Modifications

The code consists of four new files and two modifications:

#### New Files
* _includes/github-comments.html
* _sass/_gh-code.scss
* _sass/_gh-comments.scss
* js/github-comments.js

#### Modified Files
* _layouts/default.html
* _sass/minima.scss

### Reference Implementation
The repository dc25/minimaWithGithubComments is a clone of the jekyll/minima repository modified to allow Github comments.  In addition to the Github comments changes, the blog contains a single post that shares the same comments as this post.   

### Configuration

* Set, "github_comments_repository" in _config.yml to the name of the repository to use for comments.  You can either create a repository for this purpose or use an already existing one.

* Create a new issue in the repository specified in _config.yml to hold the comments for your blog post.  Github will assign it an id.  

* Set "github_comments_issueid" in front matter for a blog post to the id just assigned by Github. 


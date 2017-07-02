---
layout: post
title: "Getting newest reddit posts in RSS"
date: 2017-07-02 20:20:30 +0000
published: true
github_comments_issueid: "2"
tags:
---

Sometimes I've had trouble with reddit feeds working inside of my feed reader (feedly).  I add the feed successfully but the newest post that gets displayed is from long ago.  This may be a reddit problem or a feedly problem or a reddit/feedly compatibility problem.  It may be fixed by the time you read this post.

Through trial and error I learned that using the following format for the reddit rss feed seems to produce up to date posts:

    https://reddit.com/r/<subreddit>/.rss

That's `https` ( not `http` ), `reddit.com` ( not `www.reddit.com` ) and `.rss` ( not `new.rss` ). 

If you can shed any light on why this works ( or perhaps does not work ) I would be interested in hearing about it.



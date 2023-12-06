---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Preliminary stuff

Research Question:
Do certain subreddits exhibit a higher proportion of self-posts, and does this correlate with the level of community engagement?

Approach:

Self-Post Analysis:

Explore the is_self field in the submissions dataset to identify self-posts (text-only submissions).
Calculate the proportion of self-posts within each subreddit.
Community Engagement Metrics:

Define community engagement metrics, such as average score per post or average number of comments per post.
Analyze whether the proportion of self-posts correlates with these engagement metrics.
Visualization:

Create bar charts or scatter plots to visualize the relationship between the proportion of self-posts and community engagement metrics.

# Reddit Reacts: A Deep Dive Into Engagement of Different Types of Posts

## Abstract
Social media platforms provides an environment for communities to come together and have their members interact with each other.  How exactly does this interaction happen? On Reddit, users can post submissions or comments, and react to these with 'Upvotes' or 'Downvotes'.  Looking deeper is key to understanding how exactly online social platform users engage with certain content.  These findings are imperative to understanding how content can be manipulated to attract more community engagement for marketing, influencing or personal uses.  In this paper we will investigate how Reddit reacts to different types of posts.  We will examine whether there is more community engagement for self posts or links, and within each category how exactly Reddit users *feel* about these posts.  Within each cateogory of post we will examine how levels of community engagement fluctuate and how sentiment changes between self posts and direct links.

### Reearch Questions
1. Do certain subreddits exhibit a higher proportion of self-posts?
2. Does this correlate with the level of community engagement?

### Datasets used
Main dataset (Metadata only, curated set of subreddits, downsampled to ~1GB)

For both comments and submissions:
id: a unique id for the item
score: score of the item (upvotes minus downvotes, with some algorithmic ‘fuzzing’ applied)
author: username of the user who posted the item, can be ‘[deleted]’ if an item has been deleted from its authors’ profile, or ‘AutoModerator’ if posted by the AutoModerator bot
subreddit: name of the subreddit the item was posted in
created_utc: time the item was posted, in Unix time

For comments only:
link_id: id of the link to which this comment belongs
body: textual content of the comment, in the ‘text’ dataset only


### Methods
Self-Post Analysis:
Explore the is_self field in the submissions dataset to identify self-posts (text-only submissions).
Calculate the proportion of self-posts within each subreddit.

Community Engagement Metrics:
Define community engagement metrics, such as average score per post or average number of comments per post.
Analyze whether the proportion of self-posts correlates with these engagement metrics.

- Examine the data with basic aggregates first, look at distribution of data (posts, comments)
- Can ignore subreddits that have little to no activity for a given time period
- Examine trends throughout time, week,month,months
- Calculate proportion of self-posts within each subreddit as above
- Define community engagement metrics as above + basic analysis
- Use PCA to reduce dimensionality
- use kmeans to cluster subreddits together by levels of community engagement and color code by partisanship and also by self post
- examine clusters by:
    - size
    - shape / variance
    - density
- Do sentiment analysis on self posts
- Do sentiment analysis on comments as a whole
- See if we get better community engagement through self posts or direct links by making 2 separate groups and examining stats
- Within self posts, analyze community engagement of each type of post (categorized by sentiment)
    - use basic aggregates but also comment count and sentiment analysis of the comments themselves


# Conclusion

Redditors do not feel any significant difference between self posts and direct links.  Even more so, Redditors do not feel any difference between *types* of self posts, whether the self posts are positive, negative or neutral has no bearing on the community engagement.  Slightly interesting to note that positive self posts generally have more more comments and a lower score on average than negative self posts.
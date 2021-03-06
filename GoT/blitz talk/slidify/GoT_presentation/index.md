---
title       : Network analysis
subtitle    : of Game of Thrones family ties
author      : Shirin Glander
job         : Data Scientist @codecentric
framework   : io2012        # {io2012, html5slides, shower, dzslides, revealjs, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {selfcontained, standalone, draft}
knit        : slidify::knit2slides
logo        : logo.jpg
---

<style>
.title-slide {
  background-color: #121621; /* #EDE0CF; ; #CA9F9D*/
}
</style>

## What can network analysis tell us?

A network is a graph of interconnected nodes/vertices.

Network analysis can e.g. be used to explore relationships in social or professional networks.

These can give us a lot of information about the patterns of how people interact.

<br>

> * Who is the most connected (i.e. influential or “important”)?
> * Are there clusters of tightly connected people?
> * Are there a few key players that connect clusters of people?

--- .class #id 

## What can network analysis tell us?

A network is a graph of interconnected nodes/vertices.

Network analysis can e.g. be used to explore relationships in social or professional networks.

These can give us a lot of information about the patterns of how people interact.

<br>

- Who is the most connected (i.e. influential or “important”)?
- Are there clusters of tightly connected people?
- Are there a few key players that connect clusters of people?

<br>

# Disclaimer

Beware of spoilers for Game of Thrones Season 1 through 6!

--- &twocol



## The Game of Thrones character network

*** =left

<br>

- R version 3.4.0
- **igraph**

<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/family_tree_GoT_legend.png" style="width: 50%; height: 50%"/></center>

- nodes == characters
- node shape: gender
- node size: popularity

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-9-1.png" style="width: 85%; height: 85%"/></center>

*** =fullwidth

--- &twocol

## The Game of Thrones character network

*** =left

<br>

- R version 3.4.0
- **igraph**

<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/family_tree_GoT_legend.png" style="width: 50%; height: 50%"/></center>

- nodes == characters
- node shape: gender
- node size: popularity

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-9-1_2.png" style="width: 85%; height: 85%"/></center>

*** =fullwidth

--- &twocol

## The Game of Thrones character network

*** =left

<br>

- R version 3.4.0
- **igraph**

<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/family_tree_GoT_legend.png" style="width: 50%; height: 50%"/></center>

- nodes == characters
- node shape: gender
- node size: popularity

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-9-1_3.png" style="width: 85%; height: 85%"/></center>

*** =fullwidth

--- &twocol

## The Game of Thrones character network

*** =left

<br>

- R version 3.4.0
- **igraph**

<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/family_tree_GoT_legend.png" style="width: 50%; height: 50%"/></center>

- nodes == characters
- node shape: gender
- node size: popularity

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-9-1_4.png" style="width: 85%; height: 85%"/></center>

*** =fullwidth



--- &twocol

## Who are the most important characters?

*** =left

### Betweenness centrality

- shortest paths between nodes
- key connections or bridges between different groups of nodes

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-21-1.png" style="width: 90%; height: 90%"/></center>

*** =fullwidth



--- &twocol

## Who are the most important characters?

*** =left

### Betweenness centrality

- shortest paths between nodes
- key connections or bridges between different groups of nodes


```r
##              rowname
## 1       Eddard Stark
## 2        Sansa Stark
## 3   Tyrion Lannister
## 4    Tywin Lannister
## 5   Joanna Lannister
```

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-21-1_2.png" style="width: 90%; height: 90%"/></center>

*** =fullwidth

--- &twocol

## Who are the most important characters?

*** =left

### Betweenness centrality

- shortest paths between nodes
- key connections or bridges between different groups of nodes

<br>

- **House Stark and House Lannister are the most important family connections in Game of Thrones**

*** =right
<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/figures_post/unnamed-chunk-21-1_2.png" style="width: 90%; height: 90%"/></center>

*** =fullwidth

--- .class #id 



## Thank you!

Full code with explanations and bigger pictures at

[https://shiring.github.io/networks/2017/05/15/got_final](https://shiring.github.io/networks/2017/05/15/got_final).

Slides and code for how I generated the presentation with **slidify** will also go up on my blog

[https://shiring.github.io](https://shiring.github.io).

<br>

<center><img src="/Users/Shirin/Documents/Github/blog_posts_prep/GoT/blitz talk/map.png" style="width: 80%; height: 80%"/></center>

MünsteR User Group at [https://www.meetup.com/Munster-R-Users-Group](https://www.meetup.com/Munster-R-Users-Group).

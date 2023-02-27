---
title: 'A Fun Unsolved Problem - Covered Grids'
date: 2023-01-20
permalink: /posts/2023/01/covered-grids/
usemathjax: true
usetikzjax: true
tags:
---

I want to share a fun problem I don't know how to solve! I discovered it a few years ago, but I only got a few partial results. It also has some neat implications I’ll talk about later!

The way I like to frame this problem deals with "covered" "grids". A grid in this case is an n-by-n grid of unit squares, each of which can be colored or uncolored. An n-by-n grid is covered if each rectangle in the grid of area at least n contains a colored square. These images illustrate some examples!

<script type="text/tikz">   \begin{tikzpicture}
\draw[step=1cm,black] (0,0) grid (4,4);
\fill[black] (0,3) rectangle (1,4);
\fill[black] (1,1) rectangle (2,2);
\fill[black] (2,2) rectangle (3,3);
\fill[black] (3,0) rectangle (4,1);
  \end{tikzpicture} </script>

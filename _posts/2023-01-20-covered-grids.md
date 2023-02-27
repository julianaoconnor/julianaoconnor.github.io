---
title: 'A Fun Unsolved Problem - Covered Grids'
date: 2023-01-20
permalink: /posts/2023/01/covered-grids/
tags:
---

<head>
  <script
    src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"
    type="text/javascript">
  </script>
  <link rel="stylesheet" type="text/css" href="http://tikzjax.com/v1/fonts.css">
  <script src="http://tikzjax.com/v1/tikzjax.js">
  </script>
</head>

I want to share a fun problem I don't know how to solve! I discovered it a few years ago, but I only got a few partial results. It also has some neat implications I’ll talk about later!

Test:

$ 3 + 4 x = 5 $

The way I like to frame this problem deals with "covered" "grids". A grid in this case is an n-by-n grid of unit squares, each of which can be colored or uncolored. An n-by-n grid is covered if each rectangle in the grid of area at least n contains a colored square. These images illustrate some examples!

<script type="text/tikz">   \begin{tikzpicture}
\draw[step=1cm,black] (0,0) grid (4,4);
\fill[black] (0,3) rectangle (1,4);
\fill[black] (1,1) rectangle (2,2);
\fill[black] (2,2) rectangle (3,3);
\fill[black] (3,0) rectangle (4,1);
  \end{tikzpicture} </script>

This 4-by-4 grid is covered, as every rectangle in the grid of area at least 4 contains a colored square.

<script type="text/tikz">   \begin{tikzpicture}
\draw[step=1cm,black] (0,0) grid (4,4);
\fill[black] (0,3) rectangle (1,4);
\fill[black] (1,2) rectangle (2,3);
\fill[black] (2,1) rectangle (3,2);
\fill[black] (3,0) rectangle (4,1);
\draw[red, very thick] (2,2) rectangle (4,4);
  \end{tikzpicture} </script>

This 4-by-4 grid is not covered, as the red rectangle has an area of 4 and does not contain a colored square.

<script type="text/tikz">   \begin{tikzpicture}
\draw[step=1cm,black] (0,0) grid (5,5);
\fill[black] (0,4) rectangle (1,5);
\fill[black] (1,3) rectangle (2,4);
\fill[black] (2,2) rectangle (3,3);
\fill[black] (3,1) rectangle (4,2);
\fill[black] (4,0) rectangle (5,1);
\draw[red, very thick] (2,3) rectangle (5,5);
  \end{tikzpicture} </script>

This 5-by-5 grid is not covered, as the red rectangle has an area of 6 (and thus an area greater than 5) and does not contain a colored square.

<script type="text/tikz">   \begin{tikzpicture}
\draw[step=1cm,black] (0,0) grid (5,5);
\fill[black] (0,4) rectangle (1,5);
\fill[black] (2,3) rectangle (3,4);
\fill[black] (4,2) rectangle (5,3);
\fill[black] (1,1) rectangle (2,2);
\fill[black] (3,0) rectangle (4,1);
  \end{tikzpicture} </script>

This 5-by-5 grid is covered, as every rectangle in the grid of area at least 5 contains a colored square.

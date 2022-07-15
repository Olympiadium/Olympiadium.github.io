---
layout: article
title: LaTeX Chapter 1 Introduction to TeX | Olympiadium
date: 2021-09-10
mathjax: true
code: true
permalink: /computer-and-coding/latex/chapter-1/introduction
---
# TeX 소개
<ul class="breadcrumb">
	<li><a href="{{ site.homeurl }}">Olympiadium</a></li> 
	<li><a href="{{ site.homeurl }}computer-and-coding/">Computer and Coding</a></li> 
	<li><a href="{{ site.homeurl }}computer-and-coding/latex/">LaTeX</a></li>
	<li><a href="{{ site.homeurl }}computer-and-coding/latex/chapter-1/">Chapter 1</a></li>
	<li><a href="{{ site.homeurl }}computer-and-coding/latex/chapter-1/introduction/">TeX 소개</a></li>
</ul>

## TeX이란?
<blueboard><pre><code class="language-latex line-numbers match-braces">\NeedsTeXFormat{LaTeX2e}
\ProvidesClass{gshstest}[GSHS Test Class]
\LoadClass[11pt]{article}

\usepackage[b4paper,left=50pt,right=50pt,top=65pt,bottom=80pt,headsep=10pt]{geometry}
\usepackage{setspace}
\usepackage{graphicx}

\begin{minipage}[<i>options</i>]{<i>width</i>}
	contents here...
\end{minipage}
</code></pre>
</blueboard>
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
<blueboard><pre><code class="language-latex">\NeedsTeXFormat{LaTeX2e}
\ProvidesClass{gshstest-math}[GSHS Test Class]
\LoadClass[11pt]{article}
\usepackage[b4paper,left=50pt,right=50pt,top=65pt,bottom=80pt,headsep=10pt]{geometry}
\usepackage{setspace}
\usepackage{graphicx}
\graphicspath{ {./figures/} }
\usepackage{kotex}
\usepackage{lastpage}
\usepackage{xcolor}
\renewcommand\r[1]{\color{red}{#1}}
\newcommand\bl[1]{\color{blue}{#1}}
\usepackage{fontspec}
\usepackage{amsmath}
\usepackage{amssymb}
\usepackage{fp}
\usepackage{tikz}
\usetikzlibrary{backgrounds}
\tikzstyle{background rectangle}=[thin,draw=black]
\usepackage{environ}
\NewEnviron{tbox}[1]{%
	\\
	\begin{minipage}{\linewidth-6\fboxsep}
    	\begin{tikzpicture}[show background rectangle]
    		\node[align=justify, text width=\linewidth, inner sep=0pt]{
    			\\\BODY
    		};
    		\node[yshift=-0.7ex,overlay,fill=white,draw=white,above] at (current bounding box.north){#1};
    	\end{tikzpicture}
    \end{minipage}
}
</code></pre>
</blueboard>
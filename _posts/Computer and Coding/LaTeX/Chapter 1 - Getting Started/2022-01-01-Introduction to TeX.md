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
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/computer-and-coding/">Computer and Coding</a></li> 
	<li><a href="{{ site.baseurl }}/computer-and-coding/latex/">LaTeX</a></li>
	<li><a href="{{ site.baseurl }}/computer-and-coding/latex/chapter-1/">Chapter 1</a></li>
	<li><a href="{{ site.baseurl }}/computer-and-coding/latex/chapter-1/introduction/">TeX 소개</a></li>
</ul>

## TeX이란?
<!--<blueboard><pre style="white-space: pre-wrap;"><code class="language-latex">
	\NeedsTeXFormat{LaTeX2e}
	\ProvidesClass{gshstest}[GSHS Test Class]
	\LoadClass[11pt]{article}
	
	\usepackage[b4paper,left=50pt,right=50pt,top=65pt,bottom=80pt,headsep=10pt]	{geometry}
	\usepackage{setspace}
	\usepackage{graphicx}
	
	\begin{document}
		\begin{minipage}[<i>options</i>]{<b>width</b>}
			\begin{center}
				centered...
			\end{center}
			contents here...
		\end{minipage}
		
		\begin{tikzpicture}
			\draw[help, help lines, curve, ->, pos=mid, go=value] (0,0) grid (3,2);
			\draw (-1,0) parabola[parabola height=2cm] +(3,0);
		\end{tikzpicture}
	\end{document}
</code></pre>
</blueboard>-->
<pre style="white-space: pre-wrap;"><code class="language-cpp">
#import&lt;bits/stdc++.h&gt;  
#define o push_back  
#define s 999999  
using namespace std;int n,r,w,m,e,x,k,l,i,a[s],d[3][s],b[s];vector&lt;int&gt; v[s],c;queue&lt;int&gt; q;int f(int z){while(!q.empty()){w=q.front();q.pop();for(i=0;i&lt;v[w].size();i++){e=v[w][i];if(b[e])continue;b[e]=1;d[z][e]=d[z][w]+1;q.push(e);}}if(z==1&&!b[1]){cout&lt;&lt;"Flee";abort();}fill(b,b+s,0);}main(){cin&gt;&gt;n&gt;&gt;m&gt;&gt;x;for(i=0;i&lt;m;i++,cin&gt;&gt;k&gt;&gt;l,v[k].o(l),v[l].o(k));for(i=0;i&lt;x;)cin&gt;&gt;a[i++];q.push(1);b[1]=1;d[2][1]=0;f(2);for(i=0;i&lt;x;i++){q.push(a[i]);b[a[i]]=1;d[0][a[i]]=0;}f(0);q.push(n);b[n]=1;d[1][n]=0;f(1);c.o(d[2][n]);for(i=0;i++&lt;n;)if(d[2][i]&lt;d[0][i])c.o(d[1][i]);r=*min_element(&c[0],&c[c.size()]);cout&lt;&lt;(x?d[0][1]?r:d[1][1]+1:0);}
</code></pre>
<pre data-src="/code/TeX/chapter-1/test.tex" data-range="10,16"></pre>
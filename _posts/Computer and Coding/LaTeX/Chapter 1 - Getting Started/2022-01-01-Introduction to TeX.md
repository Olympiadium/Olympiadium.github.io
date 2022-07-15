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
\NewEnviron{bbox}{%
	\\
	\begin{minipage}{\linewidth-6\fboxsep}
		\begin{tikzpicture}[show background rectangle]
    		\node[align=justify, text width=\linewidth, inner sep=0pt]{
    			\BODY
    		};
    	\end{tikzpicture}
    \end{minipage}
}
\NewEnviron{cbox}{%
	\\[-1ex]
	\begin{minipage}{\linewidth-8\fboxsep}
		\begin{tikzpicture}[show background rectangle]
    		\node[align=justify, text width=\linewidth, inner ysep=4pt]{
    			\hspace*{\fill}\BODY\hspace*{\fill}\null
    		};
    	\end{tikzpicture}
    \end{minipage}
}
\NewEnviron{dbox}{%
	\\[-1ex]
	\begin{minipage}{\linewidth-4\fboxsep}
		\begin{tikzpicture}[show background rectangle]
    		\node[align=justify, text width=\linewidth, inner ysep=4pt]{
    			\hspace*{\fill}\BODY\hspace*{\fill}\null
    		};
    	\end{tikzpicture}
    \end{minipage}
}

\usepackage{multirow}
\usepackage{tabularx}
\renewcommand\tabularxcolumn[1]{>{\Centering}m{#1}}
\usepackage{ragged2e}
\usetikzlibrary{matrix}
\tikzset{
  grouping/.style={inner sep=2pt, baseline=0ex, left delimiter={[}},
}
\newlength\groupinglength
\setlength\groupinglength{\linewidth}
\NewEnviron{lbox}[1]{%
	\hspace*{3ex}%
	\begin{tikzpicture}
		\addtolength\groupinglength{-1ex}%
  		\node [grouping] (block) {\hspace{1ex}\parbox{\groupinglength}{\BODY}};%
  		\node[xshift=-.5\widthof{#1},overlay,fill=white,draw=white,inner sep=1pt] at (block.west) {#1};
  	\end{tikzpicture}
}


\usepackage{adjustbox}
\def\|#1\|{\ensuremath{\mathrm{#1}}}
\newcommand{\vspan}[1][1]{\vspace*{\stretch{\fpeval{10*(#1)}}}}
\usepackage{setspace}
\usepackage{boldline}
\usepackage{stackengine}
\usepackage{enumitem}
\usepackage{subfiles}
\usepackage{multicol}
\setlength{\columnseprule}{0.4pt}
\usepackage{wrapfig}

\usepackage[at]{easylist}
\ListProperties(Hang=true, Margin=5pt, Style1*=\fontspec[Path=./fonts/]{HYWULM.TTF}\selectfont,%
Style2*={(}, Mark2={)}, Numbers2=a, Hide2=1,%
Space1=1cm, Space2=0.5cm, Space2*=0.3cm, Hide3=3, Space4=0.2cm, Hide4=4)

\def\(#1\){\addstackgap{$\displaystyle#1$}}
\usepackage[per-mode=symbol]{siunitx}
\sisetup{inter-unit-product=\ensuremath{{}\cdot{}}}
\setlength\parindent{0pt}
\newcommand{\dan}{\textbf{[단답형]} }
\newcommand{\seo}{\textbf{[서술형]} }
\newcommand{\non}{\textbf{[논술형]} }
\newcommand{\sn}{\textbf{[서$\cdot$논술형]} }
\renewcommand{\u}{\underline}
\renewcommand{\i}{\textit}
\renewcommand{\b}{\textbf}

\setmainfont{HANBatang.ttf}[Path=./fonts/,BoldFont=*B,WordSpace={1.2,1.2,0}]
\title{\year학년도+\sem학기+\term차+지필평가+원안지(\subject).pdf}
\author{}
\date{}
\renewcommand{\time}{60}
\newcommand{\perfect}{100}
\newcommand\fboxed[1]{\fbox{\parbox{\dimexpr\linewidth-2\fboxsep-2\fboxrule}{#1}}}
\newcolumntype{Y}{>{\centering\arraybackslash}X}
\renewcommand{\arraystretch}{1.5}
\setlength\tabcolsep{0pt}
\setlength{\footskip}{60pt}

\usepackage{tabu}


\usepackage{fancyhdr}
\renewcommand\headrulewidth{0.4pt}
\renewcommand\footrulewidth{0.4pt}
\makeatletter % double line in header and footer
\def\headrule{{\if@fancyplain\let\headrulewidth\plainheadrulewidth\fi
		\hrule\@height\headrulewidth\@width\headwidth
		\vskip 0.8pt
		\hrule\@height.4pt\@width\headwidth
		\vskip-\headrulewidth
		\vskip-2pt}}
\def\footrule{{\if@fancyplain\let\footrulewidth\plainfootrulewidth\fi
		\hrule\@height\footrulewidth\@width\headwidth
		\vskip 0.8pt% 2pt between lines
		\hrule\@height.4pt\@width\headwidth% lower line with .5pt line width
		\vskip-\footrulewidth
}}
\makeatother


\pagestyle{fancy}
\fancyhf{}
\fancyheadoffset{0.3cm}
\fancyfootoffset{0.3cm}
\cfoot{\begin{minipage}[b]{0.95\textwidth}\begin{center}
			\vskip11.5pt%
			\fontspec[Path=./fonts/,FakeStretch=.93]{HDOTUM.TTF}\fontsize{10.9}{12}\selectfont%
			과학영재학교 경기과학고등학교\quad~~ (\subject)과~~ (\ \pageref{LastPage} )면 중 ( \thepage\ )면\quad \year학년도 \sem학기 \term차 지필평가\\
			\vskip0.35cm\fontspec[Path=./fonts/,FakeStretch=.95]{Gulim.ttf}\fontsize{7.7}{9}\selectfont%
			이 시험문제의 저작권은 경기과학고등학교에 있습니다. 저작권법에 의해 보호받는 저작물이므로 전재와 복제는 금지되며, 이를 어길시 저작권법에 의거 처벌될 수 있습니다.
\end{center}\end{minipage}}
\usepackage{dashrule}
\usepackage{listofitems}

\usepackage{multido}

\newlength\tableheight
\setlenght{\tableheight}{70pt}
\newlength\authorheight
\setlength{\authorheight}{\dimexpr\A/\authorslen\relax}

\renewcommand\maketitle{
	\begin{table}[]
		\fontspec[Path=./fonts/]{MalgunGothic-Bold.ttf}\selectfont
		\begin{tblr}{stretch=0,column{1}={8.4cm},column{2,4}={0.7cm,font=\setstretch{0.5}\fontsize{10.5}{10.5}\selectfont},column{3}={2.5cm},vlines={1.2pt},rowsep=0pt,colsep=0pt,colspec={Q[c,m]Q[c,m]Q[c,m]Q[c,m]X}}
			\hline[1.2pt]
			\begin{tblr}{stretch=0,rowsep=0pt,colsep=0pt,row{1}={abovesep=5pt},row{2}={belowsep=3pt},row{3}={font=\fontsize{12}{11}\selectfont},colspec={X[c]|X[c]|X[c]|X[c]},rowspec={Q[ht=21pt]Q[ht=21pt]Q[ht=21pt]}}
				\SetCell[c=4]{r} \fontsize{13.6}{14}\selectfont \year학년도 제\sem학기 \term차 지필평가~~~\\
				\SetCell[c=4]{r} \fontsize{13.6}{14}\selectfont {[}\subject{]}과\quad (\time분)~~~\\\hline
				학 점 & 2 & 과목 총점 & \perfect
			\end{tblr}
			& {\\[-\baselineskip-1pt]출제\\[1ex]및\\[1ex]검토}
			& \begin{tabular}{r}%{stretch=0,rowsep=0pt,colsep=0pt,rows={ht=35pt},colspec={X[r]}}
					hi \\ bye \\
					\skyIDtable
				\end{tabular}
			& {\\[-\baselineskip-2pt]결\\[2em]재} & 아 \\
			\hline[1.2pt]
		\end{tblr}
	\end{table}
	\vspace*{-1.3cm}
}

\usepackage{array}
\usepackage{tabularray}
\usepackage{mathtools}
\sisetup{group-separator={,},
	group-minimum-digits=4,}
\newcommand{\til}{\,\textasciitilde\,}
\newcommand{\colbr}{\vfill\null\columnbreak}
\newcolumntype{M}[1]{>{\centering\arraybackslash}m{#1}}
</code></pre>
</blueboard>
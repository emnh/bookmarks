# LaTeX resources
 - PGF/TikZ: Graphs and Diagrams: http://ctan.uib.no/graphics/pgf/base/doc/pgfmanual.pdf
 - xfp: Floating Point Calculation: http://ctan.uib.no/macros/latex/contrib/l3packages/xfp.pdf
 - hyperref: For hrefs.
 - import: To share preamble between files.
 - natbib: Bibliography.
 - graphicx: Insert images.
 - pgfplots: Plotting.
 - caption: Figures without float.
 - parskip: Minus indent plus spacing
 - subfiles: Compile sections standalone
 - listings: Box and color(?) source code
 - gensymb: Symbols such as \degree
 
# Preamble

```tex
\usepackage{import}
\usepackage{natbib}
\usepackage{amsmath}
\usepackage{graphicx}
\usepackage{hyperref}
\hypersetup{
    colorlinks=true,
    linkcolor=blue,
    filecolor=magenta,      
    urlcolor=cyan,
}
\usepackage{tikz}
\usepackage{pgfplots}
\usepackage{xfp}
\usepackage{caption}
\usepackage{parskip}
\usepackage{subfiles}

\usepackage{listings}
\usepackage{xcolor}
\lstset { %
    language=C++,
    backgroundcolor=\color{black!5}, % set backgroundcolor
    basicstyle=\footnotesize,% basic font setting
}
\pgfplotsset{compat=1.15}

\usepackage{gensymb}

% \usepackage{expl3}
% \ExplSyntaxOn
% \cs_new_eq:NN \fpeval \fp_eval:n
% \ExplSyntaxOff
\protected\def\fpset#1#2{\edef#1{\fpeval{#2}}}

% \usepgfplotslibrary{external}

% \tikzexternalize

\setlength\parindent{0pt}
```

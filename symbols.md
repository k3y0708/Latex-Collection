# Symbols

## Colored dots

```latex
% Colored dots
\usepackage{tikz}
\newcommand*\emptycirc[1][1ex]{\tikz\draw (0,0) circle (#1);} 
\newcommand*\halfcirc[1][1ex]{%
  \begin{tikzpicture}
  \draw[fill] (0,0)-- (90:#1) arc (90:270:#1) -- cycle ;
  \draw (0,0) circle (#1);
  \end{tikzpicture}}
\newcommand*\fullcirc[1][1ex]{\tikz\fill (0,0) circle (#1);} 
```

```latex
% With thick lines
\usepackage{tikz}
\newcommand*\emptycirc[1][1ex]{\tikz\draw[thick] (0,0) circle (#1);} 
\newcommand*\halfcirc[1][1ex]{%
  \begin{tikzpicture}
  \draw[fill] (0,0)-- (90:#1) arc (90:270:#1) -- cycle ;
  \draw[thick] (0,0) circle (#1);
  \end{tikzpicture}}
\newcommand*\fullcirc[1][1ex]{\tikz\fill (0,0) circle (#1);} 
```

```latex
% Demo of circles
\begin{tabular}{|c|}
            \hline
            \emptycirc \emptycirc[2ex]\\ \hline
            \halfcirc \halfcirc[2ex]\\ \hline
            \fullcirc \fullcirc[2ex]\\ \hline
        \end{tabular}

\end{document}
```

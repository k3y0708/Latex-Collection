# Document styling

## Prevent indent of new paragraphs

```latex
\setlength\parindent{0pt} % in Header
```

## Full page title page

```latex
% document header
\usepackage{titling}
\renewcommand\maketitlehooka{\null\mbox{}\vfill}
\renewcommand\maketitlehookd{\vfill\null}

\title{Awesome title}
\author{Best Author Ever}
\date{In the future of the past}
```

```latex
% begin of document body
\begin{titlingpage}
\maketitle
\end{titlingpage}

\newpage
```


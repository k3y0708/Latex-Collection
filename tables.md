# Tables

## Tables with line break in Cell

```latex
% Linebreak in table cell
\usepackage[utf8]{inputenc}
\usepackage{fourier}
\usepackage{array}
\usepackage{makecell}
\renewcommand\theadalign{bc}
\renewcommand\theadfont{\bfseries}
\renewcommand\theadgape{\Gape[4pt]}
\renewcommand\cellgape{\Gape[4pt]}
```

```latex
% in Cell
\makecell{Funny text \\ with linebreak}
```


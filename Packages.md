# Packages

* Imágenes [ver más](http://www.kwasan.kyoto-u.ac.jp/solarb6/usinggraphicx.pdf):

```Latex
\usepackage{graphicx}
```


* Enumeraciones [ver más](https://tex.stackexchange.com/questions/121042/enumerate-package):

```Latex
\usepackage{enumerate}
\usepackage{enumitem}
```

* Unicode and Extra characters:

```Latex
\usepackage[utf8]{inputenc}
```

* Espacios en parrafos y formato:

```Latex
\usepackage{setspace}
```

* Formato para Algoritmos [ver más](http://ctan.math.washington.edu/tex-archive/macros/latex/contrib/algorithms/algorithms.pdf):

```Latex
\usepackage[]{algorithm2e}
```

Ejemplo:

```Latex
\begin{algorithm}[H]
 \KwData{this text}
 \KwResult{how to write algorithm with \LaTeX2e }
 initialization\;
 \While{not at end of this document}{
  read current\;
  \eIf{understand}{
   go to next section\;
   current section becomes this one\;
   }{
   go back to the beginning of current section\;
  }
 }
 \caption{How to write algorithms}
\end{algorithm}
```
# Código de ayuda para Latex

Iniciamos el documento con:
```Latex
\documentclass[12pt]{article}
```
Especificamos paquetes:

```Latex
\usepackage{amsfonts}
\usepackage[top=1in, bottom=1in, left=1in, right=1in]{geometry}
\usepackage{amsfonts}
\usepackage{graphicx}
\usepackage{enumerate}
\usepackage[utf8]{inputenc}
\usepackage{setspace}
\usepackage[]{algorithm2e}

```
Definimos macros o ecuaciones que usaremos a lo largo del documento
```Latex
\def\eq1{y=\frac{x}{x^2+3x+2}}
```

Iniciamos documento...
```Latex
\begin{document}
```

Indicamos Indice:
```Latex
% Indice, automaticamente pone los sections y subsections
\tableofcontents
```

Ponemos titulo, autor y fecha...
```Latex
\title{MiTitulo}
\author{Richie}
% Poner fecha de hoy
\date{\today}
% Quitar fecha
\date{\small{}}
\maketitle
```
Ponemos Secciones y subsecciones...
```Latex
\section{Seccion uno (20 pts)}
\subsection{Subseccion}
\subsection{Subseccion}
\section{Seccion dos}
\subsection{Subseccion}
```
Estilo en texto:
```Latex

My text \textit{italiano} texto.
Ahora es \textbf{negro}.
Y ahora es  \textsc{MAYUSCULAS}.
Y ahora escrito por un  \texttt{typewriter} \\
Soy un sitio web \texttt{http://www.google.com.mx}\\

Usando Macros, una ecuaciÃ³n definida arriba: $\eq1$
\\
letras grandes \begin{Large}
holaaaaa
\end{Large}

texto \begin{center}
centrado
\end{center}

Texto justificado 
\begin{flushleft}
texto texto texto
\end{flushleft}
```

Lenguaje Matemático:
```Latex
Numeros naturales $\mathbb{N}$, gracias al paquete "amsfonts".
$\mathbb{Z}$

Hola que hace $(x+1)$ and $(x+3)$\\

supperscripts:
$$ 2x^2$$
$$ 2x^{3x+4}$$

subscripts:
$$x_1$$
$$x_{12}$$
$${{x_1}_2}_3$$

trig functions:
$$y=\sin{x}$$

log functions:
$$\log{x}$$
$$\ln{x}$$

square roots:
$$\sqrt[3]{x^{3x+2}}$$

fractions:\\
About $\frac{2}{3}$ of the glass if full.\\
\\
Fracciones mas grandes $\displaystyle{\frac{2}{3}}$ of the glass if full.

$$\frac{x}{x^2+x+1}$$

Parentesis:
$$\{a,b,c,d,e\}$$

$$3\left(\frac{2}{3}\right)$$

$$3\left[\frac{2}{3}\right]$$

$$3\left\{\frac{2}{3}\right\}$$

$$\left. \frac{dy}{dx} \right|_{x=1}$$
```

Tablas:
```Latex
Tables, c una columna, cc dos columnas...\\
con ampersan cambiamos de columna.\\

\begin{tabular}{|c|ccccc|}
\hline
$x$  & 1 & 2 & 3 & 4 & 5 \\ \hline
$f(x)$  & 11 & 22 & 33 & 43 & 54 \\ \hline
\end{tabular}

Ecuaciones, con amperson se alinean los = :
El asterisco oculta los indices de la derecha
\begin{eqnarray*}
5x^2-9 &=& x + 3 \\
3x^2-9 &=& 12 \\
5x^2-9 &=& x + 3\\
x&\approx&\pm1.2323
\end{eqnarray*}
```

Enumeraciones:
```Latex 
Enumeraciones:
\begin{enumerate}
\item Pencil
\item calculator
\item ruler
	\begin{enumerate}
	\item adasdads
	\begin{enumerate}
	\item adasdads
	\end{enumerate}
	\item adsdsdsd
	\item adsdsdsd
	\end{enumerate}
\item graph
\end{enumerate}
```

Incisos:
```Latex
\begin{enumerate}[6)]
	\item Respuesta:
	% Inciso a)
	\begin{enumerate}[a)]
	\item La función sería $O(n^2)$
	\end{enumerate}
	
	% Inciso b)
	\begin{enumerate}[b)]
	\item La función sería $\Omega(n^2)$
	\end{enumerate}
	
	% Inciso c)
	\begin{enumerate}[c)]
	\item El algoritmo seria el siguiente:
	
	    \hspace{15pt} var $j = Null$
	    
		\hspace{15pt} For $i = 1,2,..., n$
		
		\hspace{35pt} $j +=  i+ 1$
		
		\hspace{35pt} $B[i,j] = $ Add up $A[i]$ through $A[j]$
		
		\hspace{15pt} End
		
	\end{enumerate}
\end{enumerate}
```

Imagenes:
```Latex
\includegraphics[width=5in]{imagen.png}
```

Fin del documento:
```Latex
\end{document}
```

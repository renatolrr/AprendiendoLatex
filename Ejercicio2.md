#Cómo escribir una tesis con LaTeX  
  
##Comienzo  
  
´´´
\documentclass[a4paper,openright,12pt]{book}
\usepackage[spanish]{babel}
\usepackage[latin1]{inputenc}

\begin{document}

\end{document}

```
  
##Título  
  
```
\begin{titlepage}
\begin{center}
\begin{Huge}
\textsc{Un buen título es muy importante}
\end{Huge}
\end{center}
\end{titlepage}
```
  
##Página en blanco sin numerar  
  
´´´
\newpage
$\ $
\thispagestyle{empty} % para que no se numere esta pagina  
```
  
##Dedicatoria  
  
```
\chapter*{}
\pagenumbering{Roman} % para comenzar la numeracion de paginas en numeros romanos
\begin{flushright}
\textit{Dedicado a \\
mi familia}
\end{flushright}
```
  
##Agradecimientos y Resumen
  
```
\chapter*{Agradecimientos} % si no queremos que añada la palabra "Capitulo"
\addcontentsline{toc}{chapter}{Agradecimientos} % si queremos que aparezca en el índice
\markboth{AGRADECIMIENTOS}{AGRADECIMIENTOS} % encabezado
 
¡Muchas gracias a todos!

\chapter*{Resumen} % si no queremos que añada la palabra "Capitulo"
\addcontentsline{toc}{section}{Resumen} % si queremos que aparezca en el índice
\markboth{RESUMEN}{RESUMEN} % encabezado

Una bonita historia
```
  
##Indice de contenidos, figuras y tablas  
  
```
 \tableofcontents % indice de contenidos

\cleardoublepage
\addcontentsline{toc}{chapter}{Lista de figuras} % para que aparezca en el indice de contenidos
\listoffigures % indice de figuras

\cleardoublepage
\addcontentsline{toc}{chapter}{Lista de tablas} % para que aparezca en el indice de contenidos
\listoftables % indice de tablas
```
  
##Capítulos  
  
```
\chapter{Introducción}\label{cap.introduccion}
\pagenumbering{arabic} % para empezar la numeración con números
Érase una vez...
\section{sección1}
Bla bla bla
\subsection{subsección1}
Ble ble ble
\subsubsection{subsubsección1}
Bli bli bli
\paragraph{párrafo1}
Blo blo blo
```
  
##Apéndices  
  
```
\appendix
\chapter{Más cosas}\label{aped.A}
Aún faltan cosas por decir.

\chapter{Y más cosas aún}\label{aped.B}
Y más cosas aún.
```
  
##Bibliografía
  
```
\cleardoublepage
\addcontentsline{toc}{chapter}{Bibliografía}
\bibliographystyle{acm} % estilo de la bibliografía.
\bibliography{yyyy} % yyyy.bib es el fichero donde está salvada la bibliografía.
```
  
   
##Todo
  
```
 \documentclass[a4paper,openright,12pt]{book}
\usepackage[spanish]{babel}
\usepackage[utf8]{inputenc} 

\setcounter{secnumdepth}{3} %para que ponga 1.1.1.1 en subsubsecciones
\setcounter{tocdepth}{3} % para que ponga subsubsecciones en el indice

\begin{document}

\begin{titlepage}
\begin{center}
\begin{Huge}
\textsc{Un buen título es muy importante}
\end{Huge}
\end{center}
\end{titlepage}

% para crear una cara en blanco
\newpage
$\ $
\thispagestyle{empty} % para que no se numere esta página

\chapter*{}
\pagenumbering{Roman} % para comenzar la numeración de paginas en números romanos
\begin{flushright}
\textit{Dedicado a \\
mi familia}
\end{flushright}

\chapter*{Agradecimientos} % si no queremos que añada la palabra "Capitulo"
\addcontentsline{toc}{chapter}{Agradecimientos} % si queremos que aparezca en el índice
\markboth{AGRADECIMIENTOS}{AGRADECIMIENTOS} % encabezado

¡Muchas gracias a todos!

\chapter*{Resumen} % si no queremos que añada la palabra "Capitulo"
\addcontentsline{toc}{chapter}{Resumen} % si queremos que aparezca en el índice
\markboth{RESUMEN}{RESUMEN} % encabezado

Se trata de una bonita historia.

\tableofcontents % indice de contenidos

\cleardoublepage
\addcontentsline{toc}{chapter}{Lista de figuras} % para que aparezca en el indice de contenidos
\listoffigures % indice de figuras

\cleardoublepage
\addcontentsline{toc}{chapter}{Lista de tablas} % para que aparezca en el indice de contenidos
\listoftables % indice de tablas

\chapter{Introducción}\label{cap.introduccion}
\pagenumbering{arabic}
Érase una vez...
\section{sección1}
Bla bla bla
\subsection{subsección1}
Ble ble ble
\subsubsection{subsubsección1}
Bli bli bli
\paragraph{párrafo1}
Blo blo blo

\chapter{Nudo}\label{cap.nudo}
La historia continúa con...

\chapter{Desenlace}\label{cap.desenlace}
El final de la historia es sorprendete...

\appendix
\chapter{Más cosas}\label{aped.A}
Aún faltan cosas por decir.

\chapter{Y más cosas aún}\label{aped.B}
Y más cosas aún.

\cleardoublepage
\addcontentsline{toc}{chapter}{Bibliografía}
\bibliographystyle{acm} % estilo de la bibliografía.
\bibliography{yyyy} % yyyy.bib es el fichero donde está salvada la bibliografía.

\end{document}

```
  
Fuente: http://minisconlatex.blogspot.fr

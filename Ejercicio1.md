#Cómo escribir un artículo de dos columnas con abstract, figuras y tablas en una columna  
  
##Inicio documento
```
\documentclass[a4paper,twocolumn,10pt]{article}
\usepackage[spanish]{babel}
\usepackage[latin1]{inputenc}
\usepackage{graphicx}
\usepackage{flushend}

\begin{document}

\end{document}
```  
  
##Cuerpo  
  
```
\title{Primeros días en el Paraíso}
\author{Adan y Eva}
\date{}

\twocolumn[
\begin{@twocolumnfalse}
\maketitle
\begin{abstract}
Un artículo suele empezarse con un resumen. Dicho resumen debe ser claro y conciso, y no tiene que tener referencias bibliográficas. En inglés, abstract significa resumen, y resume significa reanudar. Cuidado no confundas esas dos palabras.\\ \\
Palabras clave: Manzana, Serpiente.
\end{abstract}
\end{@twocolumnfalse}
]

\section{Introducción}

```

##Mejoras  
  
```
\twocolumn[
\begin{@twocolumnfalse}
\maketitle
\vspace*{-1cm}
\begin{center}\rule{0.9\textwidth}{0.1mm} \end{center}
\begin{abstract}
\normalsize Un artículo suele empezarse con un resumen. Dicho resumen debe ser claro y conciso, y no tiene que tener referencias bibliográficas. En inglés, abstract significa resumen, y resume significa reanudar. Cuidado no confundas esas dos palabras.\\ \\
Palabras clave: Manzana, Serpiente.
\begin{center}\rule{0.9\textwidth}{0.1mm} \end{center}
\vspace*{0.5cm}
\end{abstract}
\end{@twocolumnfalse}
]

```  
  
##Tablas y figuras  
  
```
\begin{table*}[htb]
\centering
\begin{tabular}{p{0.2\textwidth} p{0.7\textwidth}}
\hline
Montaña & Descripción \\
\hline \hline
Monte Elbrus & Se encuentra en Rusia, muy cerca de Georgia. Es la montana más alta de Europa. \\
\hline
Mont Blanc & Se encuentra en la frontera entre Francia e Italia. Erróneamente, suele decirse que es la más alta de Europa. \\
\hline
\end{tabular}
\caption{Montañas.}
\label{tabla:montanas}
\end{table*}

\begin{figure*}[htb]
\centering
\includegraphics[width=1\textwidth]{./montblanc}
\caption{Mont Blanc.}
\label{fig:mont}
\end{figure*}
```
Fuente: http://minisconlatex.blogspot.fr
  
   
 

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
 

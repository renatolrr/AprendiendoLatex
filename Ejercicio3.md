#Cómo escribir la portada de tu tesis con LaTeX  
  
```
\documentclass[a4paper,openright,12pt]{report}
\usepackage[spanish]{babel} % espanol
\usepackage[latin1]{inputenc} % acentos sin codigo
\usepackage{graphicx} % graficos

\begin{document}

\begin{titlepage}

\begin{center}
\vspace*{-1in}
\begin{figure}[htb]
\begin{center}
\includegraphics[width=8cm]{./figuras/logo}
\end{center}
\end{figure}

FACULTAD DE...\\
\vspace*{0.15in}
DEPARTAMENTO DE... \\
\vspace*{0.6in}
\begin{large}
PHD THESIS:\\
\end{large}
\vspace*{0.2in}
\begin{Large}
\textbf{EL TÍTULO DE LA TESIS ES MUY IMPORTANTE, ASÍ QUE, NO OLVIDES PONER UNO QUE SEA INTERESANTE Y ADECUADO PARA TU TESIS} \\
\end{Large}
\vspace*{0.3in}
\begin{large}
A Thesis submitted by Amy Wong for the degree of Doctor of Philosophy in the Mars University\\
\end{large}
\vspace*{0.3in}
\rule{80mm}{0.1mm}\\
\vspace*{0.1in}
\begin{large}
Supervised by: \\
Hubert J. Farnsworth \\
\end{large}
\end{center}

\end{titlepage}

\end{document}
```

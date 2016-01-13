
#El entorno multicolumn  
  
Dentro de un entorno tabulado tabular podemos agrupar varias columnas en una sola indicándole
 el formato con la orden:

```
\multicolumn{col}{formato}{contenido}
```

donde:  
  
col     número de columnas a agrupar
formato formato de la columna: l,r,c y |
  
Veamos un ejemplo:  
  
```
\begin{tabular}{|r|r|r|r|r|r|r|}
\hline \multicolumn{5}{|c|}{Semana Laboral} &
\multicolumn{2}{|c|}{Fin de semana} \\ \hline
Lunes & Martes & Miércoles & Jueves & Viernes & Sábado & Domingo \\ \hline
M & T & M & M & M & M & T \\ \hline
\end{tabular}
```

#Tabla Latex 5
```
\begin{tabular}{| l | c | r |}
	\hline
	\multirow{2}{*}{Celdas 11 y 21}	& Celda 12 & \multirow{3}{3cm}{Celdas 13, 23 y 33}	\\
	\cline{2-2}
				&	\multirow{2}{*}{Celdas 22 y 32}	&		\\
	\cline{1-1}
	Celda 31	&				&		\\
	\hline
\end{tabular}
```
  
#Tabla duda  
```
\begin{tabular}{c | c | c|}
\hline
\multicolumn{1}{|c |}{Celda 11} & Celda 12 & Celda 13 \\
\hline
Celda 21 & Celda 22 & Celda 23\\
\cline{2-3}
\end{tabular}

```

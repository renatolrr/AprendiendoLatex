
El entorno multicolumn  
  
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

#Instalar un paquete LaTeX manualmente  
  
1. Digamos que queremos el paquete algorithms (http://www.ctan.org/tex-archive/macros/latex/contrib/algorithms/).
 Nos descargamos el archivo zip.
  
2. Si el paquete que queremos viene con un archivo .sty entonces el trabajo ya está hecho,
 solo tenemos que copiar la carpeta descargada en la ruta /usr/share/texmf-dist/tex/latex/
  
3. Sin embargo, en el caso del paquete algorithms, no tenemos el archivo .sty por lo que necesitaremos compilar 
el archivo .ins, el cual creará el archivo .sty. Luego de compilar y generar el archivo .sty sólo nos quedará 
copiar la carpeta en la ruta /usr/share/texmf-dist/tex/latex/3. Finalmente sólo debemos actualizar la base de datos de latex.
  
4. Finalmente sólo debemos actualizar la base de datos de latex.  
```
mktexlsr
```
  
Nota:  
  
El lugar exacto en el que deben colocarse los nuevos archivos de estilo depende de la distribución TeX que se esté utilizando. 
Asumiendo que se utiliza una de las distribuciones modernas que son conformes al TDS (por ejemplo, TeX Live, teTeX, fpTeX o mikTeX) 
hay una serie de normas que deben tenerse en cuenta.  
  
Instalar siempre los nuevos archivos personales en una rama texmf local del árbol global o en una rama personal, 
dependiendo de si son archivos para uso común en la máquina o únicamente para el usuario. 
De esta forma puede actualizarse el árbol oficial sin tocar los archivos locales o personales. Para la rama local, 
el directorio raíz local tendrá un nombre del tipo:  
```
        texlive (win):  c:\texmf-local\
        texlive (unix): /usr/local/share/texmf/
        fpTeX:          c:\fptex\texmf.local\
        mikTeX:         c:\localtexmf\
```                          
que puede cambiar dependiendo de las opciones dadas durante la instalación o de las peculiaridades de la distribución concreta. 
Por simplicidad en lo que sigue le denominaremos $TEXMFLOCAL. 
En la rama local, reproducir la estructura de directorios de la rama principal. 
Estos son unos ejemplos de dónde deberían colocarse archivos de distintas extensiones:  
```
        .sty, .cls o .fd: $TEXMFLOCAL/tex/latex/<paquete>/
        .dvi, .ps o .pdf: $TEXMFLOCAL/doc/latex/<paquete>/
        .bib:             $TEXMFLOCAL/doc/bibtex/bib
        .bst:             $TEXMFLOCAL/doc/bibtex/bst
        .tfm:             $TEXMFLOCAL/fonts/tfm/<suministrador>/<fuente>/
        .vf:              $TEXMFLOCAL/fonts/vf/<suministrador>/<fuente>/
        .afm:             $TEXMFLOCAL/fonts/afm/<suministrador>/<fuente>/
        .pfb:             $TEXMFLOCAL/fonts/type1/<suministrador>/<fuente>/
        .ttf:             $TEXMFLOCAL/fonts/truetype/<suministrador>/<fuente>/
```
donde paquete, fuente y suministrador dependen de cada archivo individual de cada paquete.  
  
Fuente: 
http://www.aq.upm.es/Departamentos/Fisica/agmartin/webpublico/latex/FAQ-CervanTeX/FAQ-CervanTeX-8.html#ss8.1  
http://drankez.blogspot.com.es/2013/07/linux-instalar-un-paquete-latex.html  

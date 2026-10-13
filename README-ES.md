# Materiales para Mac v1

Para la revisión de principiantes en Mac de *Git & GitHub para computación y escritura científica*.
Descomprime en Descargas, fuera del proyecto. Son materiales para copiar, no un repositorio para clonar.
No copies el paquete entero al proyecto. No contiene automatización de Git ni historial.

## Etapas

- Lab 2: empieza con una carpeta nueva. Copia README.md, después .gitignore y luego requirements.txt conforme aparezcan en el libro. Finder muestra archivos ocultos con Mayúsculas-Comando-punto.
- Lab 3: copia theory/derivation.md y src/analytical.py en sus pasos respectivos. La validación de dos líneas del paso 3.6 sigue siendo una edición manual pequeña.
- Lab 4: step02 contiene el solver ejecutable; step03, la verificación de tres casos; step04, el ejecutor. Copia solo el archivo actual a src. Los scripts generan sus salidas; estas no vienen en el paquete.
- Lab 5: agrega readme-run.md al final del README. Conserva el planteamiento original.
- Lab 7: copia warmer-end.md a notes después del experimento con el extremo caliente, no antes.
- Lab 9: inserta las dos líneas de new-cases.txt al final de CASES, justo antes del corchete de cierre. Conserva los tres casos existentes.
- Lab 11: step03 es texto para agregar al final de theory/derivation.md. Los pasos 04–07 reemplazan exactamente un archivo de src cada uno. Verifica y haz commit después de cada paso. Step08 se agrega al final del README; identifica el caso anterior como v1.0. El ejecutor preparado presupone el caso del Lab 10: 101 nodos y frontera derecha a 30 C.
- Lab 12: copia step01 a una carpeta nueva kepler-orbits, incluidos .gitignore y .latexmkrc. Registra tu propio requirements-lock.txt después de instalar; no se incluye un lock específico de otra plataforma.

## Texto y figuras del Lab 12

`sections/section-00.tex` es Introduction; 01–13 corresponden a las secciones numeradas; 14 es Summary. Contienen solo el cuerpo de cada sección. Reemplaza su `% TODO`, conservando el encabezado y todas las demás secciones. El texto del artículo está en inglés en ambas ediciones.

Step05 aporta generate_kepler_data.py para la raíz. Step07 aporta los scripts de figuras 1–4 y sus bloques LaTeX. Copia un script a figures, ejecútalo y reemplaza su marcador `% FIGURE N` por el bloque correspondiente. No copies los archivos de bloques al proyecto: pega su contenido en main.tex.

Step12 aporta figuras 5–6 y adiciones de revisión. Agrega third-law-addition.tex al final de la sección 10 y variation-addition.tex al final de la 12; reemplaza sus marcadores de figura. Copia plot-notes.txt y refs.bib a la raíz. Reemplaza la línea `classical problems of mechanics.` de la introducción por citation.txt; inserta bibliography.tex justo antes de `\end{document}`. Step14 aporta la oración resuelta para el conflicto previsto.

`python build_figures.py` ejecuta solo los scripts numerados presentes en la revisión actual. `python check_data.py` comprueba el CSV orbital. `latexmk main.tex` usa .latexmkrc para generar build/main.pdf. Ninguno realiza operaciones Git. Ejecútalos desde la raíz del proyecto con su entorno virtual activo. MacTeX aporta latexmk.

## Comprobaciones

Lab 4: tres líneas PASS y punto medio 60.0 C. Lab 9: cinco líneas PASS.
Lab 11: cinco PASS después de pasos 4–5, ocho después del 6; punto medio 75.0 C tras el 7.
Lab 12: 721 muestras orbitales con radios 0.4–1.6; cuatro figuras en v1.0-submitted y seis en v1.1-revised.

Si un archivo difiere, revisa git diff antes de reemplazarlo. Detente ante resultados inesperados. La guía de recuperación empieza con un respaldo externo. No restablezcas una rama compartida para hacerla coincidir con estos materiales.

Las soluciones históricas completas siguen en https://github.com/noctis-oss/heat-transfer-1d y https://github.com/noctis-oss/kepler-orbits. Son independientes de este paquete inicial. Sus IDs de commit no son criterios de aceptación para tu repositorio.

## Reutilización

Copyright 2026 Yonatan Ali Rodríguez Arias. Puedes usar, copiar y adaptar el código y los textos de ejercicio preparados en tus propios proyectos, conforme al permiso de los listados del libro. manifest.json registra los SHA-256 de los archivos incluidos.

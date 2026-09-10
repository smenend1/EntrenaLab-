TRAINLAB PRO PWA · VERSIÓN 4
1. Sube index.html, manifest.json, sw.js, icon-192.png e icon-512.png a GitHub Pages, Netlify o tu hosting HTTPS (sustituye a todos los archivos anteriores, incluido enhanced.js que ya no existe).
2. Abre la web desde el móvil y usa "Añadir a pantalla de inicio".
3. Tus datos actuales NO se pierden: se usa la misma clave de almacenamiento local que la versión anterior.
4. Si el navegador no muestra los cambios tras publicar, borra la app de la pantalla de inicio y vuelve a añadirla (el service worker se ha renovado a v4).

CAMBIOS EN ESTA VERSIÓN respecto a v3:
- Seguridad: las notas de entrenamiento y otros textos ya no se insertan sin escapar (se corrige un riesgo de XSS al importar copias de seguridad).
- Todos los campos numéricos aceptan coma o punto decimal (10,5 y 10.5 funcionan igual).
- Validación de rangos razonables en RPE, FC, cadencia, VO2max, sueño y demás campos de recuperación, con aviso si algo se ha ajustado.
- Etiquetas de formulario ahora vinculadas a su campo (accesibilidad táctil).
- La carga (sRPE, monotony, strain, aguda/crónica) se calcula solo con sesiones de running/trail/ciclismo/caminar. Las sesiones de fuerza se muestran aparte, sin distorsionar el ACWR de resistencia.
- Nuevo: zonas de potencia de carrera (Z1-Z5) a partir de tu FTP de running, que puedes indicar en Perfil. Si no lo tienes, la app sugiere una estimación orientativa a partir de tus sesiones de tempo/competición.
- Mejores marcas separadas en "Asfalto/pista" y "Trail/desnivel notable", para no comparar tiempos de terrenos muy distintos.
- Código unificado en un único script (ya no hay archivo enhanced.js parcheando al principal), más fácil de mantener a futuro.

Las recomendaciones son orientativas y no sustituyen una valoración médica.

# Wikimedia con docker #
Este es un poyecto donde se instala wikimedia con docker y se sobre esciben algunas hojas de estilo para colorear el codigo de, por ejemplo "demo-wiki-page.html"

Sera necesario seguir los pasos de la wikimedia y habilitar 
```
wfLoadExtension( 'SyntaxHighlight_GeSHi' );
```

en el archivo 
```
LocalSettings.php
```
que te dara el sistema.

## Atencion ##

En los servidores que ofrecen hosting gratuito resulta dificil instalar debido a varias cosas.

- Son muchos archivos (serca de 20k) y con FTP se tarda mucho tiempo en subirlos.
- Si se sube archivos comprimidos para luego descomprimirlos, no se descomprimen todos los archivos.
- Dado el caso, habria que remapear los inports o requires del index.php
- la version requerida de PHP para la ultima version de Wikimedia es 7.3 y no todos los servidores ofrecen esa version.
- Si se usa la version descargable hay que ejecutar 'composer install'
- si se usa la version de docker no se puede ejecutar gratuitamente en ningun servidor.


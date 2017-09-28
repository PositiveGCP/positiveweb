# Positive WebPage (positiveweb)

Página oficial de Positive Compliance

## Construido con:

* [Materialize](http://materializecss.com) - El marco de referencia utilizado para construir la pgina
* [Bower](https://bower.io) - Manejo de dependencias.

### Arquitectura

```
- positiveweb
- mailDev
- public_html
  |- (syml) positiveweb/*
  |- (syml) mailDev
```

Como se puede observar arriba, existen dos carpetas importantes para que los servicios en este servidor sigan funcionando correctamente tales como web y correo para notificaciones automáticamente. Lo anterior se logró gracias a symlink:

Dentro de public_html

```
ln -s ../positiveweb/* .
ln -s ../mailDev .
```

### Instalación

Dentro del servidor carpeta de /positiveweb, se tendrá que ejecutar (para obtener la última versión):

```
git pull
```

### Mantenimiento

Después de que se instale la nueva versión se tendría que verificar si el servidor está respondiendo a los servicios de correo (dentro de mailDev) en la carpeta de public_html. 

## Authors

* **Dante Bazaldua** - *Trabajo inicial* - [danteese](https://github.com/danteese)
* **Tania Ubaldo** - *Diseño UX|UI* - [TaniaUba](https://github.com/TaniaUba)


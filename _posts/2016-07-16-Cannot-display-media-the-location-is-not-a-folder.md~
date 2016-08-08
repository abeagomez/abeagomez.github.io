---
layout: post
title:  "Cannot display /media/... the location is not a folder"
excerpt: "The One donde no podía ver mi disco externo"
date:   2016-07-16 19:57:19
categories: [linux]
comments: true
---
Hoy migramos mi Linux íntegramente de una máquina a otra. Sería ingenuo pensar que esto no traería consigo inconsistencias. Una de las primeras ha sido que el File Manager no era capaz de mostrar el contenido de mi disco externo, lanzando el siguiente error:


>Cannot display /media/... the location is not a folder.


El disco se montaba al conectarlo y, si accedía como root, podía ver desde la terminal que todo estaba en orden. Al haber trasladado Linux íntegramente, mi username continuó siendo el mismo.


Solución:

acceder como root a /media y eliminar el directorio que tiene por nombre tu nombre de usuario. Cuando conectes el disco duro el directorio volverá a crearse. (Esta solución funciona también si obtienes el mismo error al intentar acceder a una de las particiones internas visibles desde Linux)


>root@mipc:/# cd /media/

>root@mypc:/media# rm -rf username


Causa:

Hasta solo puedo asumir que el cambio de laptop causó alguna clase de inconsistencia en el fichero. Pero seguiré investigando y daré alguna argumentación más coherente en este apartado ;)

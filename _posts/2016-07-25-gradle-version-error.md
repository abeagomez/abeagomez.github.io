---
layout: post
title:  "Error:(1, 0) Plugin is too old, please update to a more recent version, or set ANDROID_DAILY_OVERRIDE environment variable to..."
excerpt: "The One with the gradle's wrong version"
date:   2016-07-25 23:52:10
categories: [Android]
comments: true
---
Hoy fui emocionada a empezar un nuevo proyecto en AndroidStudio cuando me encontré con el siguiente suceso:

>Error:(1, 0) Plugin is too old, please update to a more recent version, or set ANDROID_DAILY_OVERRIDE environment variable to "d6d5ee52793552d5cbc0a5c5ef6bed9e414404e4"

><a href="fixGradleElements">Fix plugin version and sync project</a><br>
><a href="openFile:/home/amy/AndroidStudioProjects/GDtect/app/build.gradle">Open File</a>

Leyendo con calma aparentemente era un problema con la versión del gradle.

Hay una solución evidente para el asunto: actualizar a una versión más reciente. Los pasos recomendados para esta actividad son:

- 1- Dentro de la carpeta que contiene el proyecto editar el fichero "build.gradle" y en la línea que dice:
classpath 'com.android.tools.build:gradle:2.2.0-alpha1'
Sustituir "2.2.0-alpha1" por una versión más reciente.

- 2- Ir a la carpeta gradle/wrapper y editar el fichero gradle-wrapper.properties para que contenga la siguiente línea:

 >distributionUrl=https\://services.gradle.org/distributions/gradle-2.10-all.zip

Claro que, aunque esa es la solución ideal, a mí no me convenció. Mi AndroidStudio funcionaba perfectamente la semana pasada! Así que tras mucho pensar, solo pude recordar que mi máquina tuvo algunos problemas con la hora. El cambio más significativo fue el año, que desde la operación de cerebro del post anterior se había quedado en 2015. 

Hice el experimento, cambié de 2016 a 2015, le dije al AndroidStudio "try again"...
Como por arte de magia, todo volvió a funcionar. Sigo pensando que lo mejor sería actualizar el gradle, pero, si como yo, se encuentran limitados de internet, asegúrense de no haber cambiado el año recientemente ;)


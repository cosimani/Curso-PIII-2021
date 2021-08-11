.. -*- coding: utf-8 -*-

.. _rcs_subversion:

Clase 01 - PIII 2021
====================
(Fecha: 11 de agosto)

:Profesores: César Osimani - Martín Salamero
:Correos: cesarosimani@gmail.com - martin.salamero@gmail.com

:Temas principales:
	- Herramientas de programación de un sistema de computadoras
	- Programación a bajo y alto nivel para el desarrollo de aplicaciones de telecomunicaciones
	- Resolución de problemas con la programación
	- Dispositivos programables
	- Tratamiento de señales en sistemas embebidos
	- Técnicas de programación avanzadas para sistemas de comunicaciones


Metodología didáctica
=====================

- A continuación se resume el conjunto de estrategias, procedimientos y acciones para facilitar el aprendizaje y el logro de nuestros objetivos. 

:Teoría: 
	- Cada clase desde las 17 horas hasta las 17:45 horas se expondrán contenidos teóricos y prácticos por parte del docente.

:Práctica: 
	- Cada clase desde las 17:45 horas estará destinado a la resolución y entrega de ejercicios "cortos".
	- El docente propone un ejercicio "corto" que, si los contenidos de la materia se mantienen al día, se pueden realizar en 20 minutos.
	- La búsqueda de la resolución del ejercicio se realiza de manera grupal en las mesas de Discord y la entrega es individual.
	- Luego de resolver el ejercicio se debe explicar oralmente durante la clase o también se puede entregar un video compartiendo pantalla explicando la resolución.
	- Para cada ejercicio se definirá un "Punto de partida" que indicará desde dónde debe comenzar la explicación.
	- Los ejecicios entregados correctamente llevan la nota 10.
	- Ejercicios no entregados llevan nota 0.
	- Ejercicios que no respeten el punto de partida y/o la completitud del ejercicio llevan nota 5.
	- Debido a que puede suceder que alguien no pueda asistir a alguna de las clases se da tiempo para la entrega del ejercicio hasta la medianoche del mismo día. En caso de necesitar más tiempo por razones particulares, escribir al docente por WhatsApp para fijar una nueva hora de entrega. Pasado este tiempo, el ejercicio queda como no entregado.
	- El video debe quedar disponible en Youtube como No listado y se comparte el link por mensaje privado en Teams.
	- Para subir videos largos a Youtube, la cuenta debe estar verificada (`ver cómo hacerlo en este video: <https://www.youtube.com/watch?v=L2BZQlnlc5M>`_)
	- Denominaremos a estos ejercicios como Entregables.
	- El tiempo de duración del video queda a criterio de quien lo entrega.
	- El video se puede editar con Blender u otro aplicativo si lo desea. (`aquí una herramienta online <https://online-video-cutter.com/es/>`_)
	- Entrar al siguiente `link para ver el registro de los entregables <https://docs.google.com/spreadsheets/d/1Qpp9mmUwuIUEbvrd_oqsQGuPOO9i1YPlHa_wBWTS6co/edit?usp=sharing>`_ 


:Regularidad: 
	- Primer nota parcial (guía de trabajos prácticos de Martín con Simulink)

	- Segunda nota parcial (Entregables de César con Python)

	- Recuperatorios: Se pueden recuperar ambos parciales durante la última semana de cursado. Completando la entrega de los prácticos de Martín o realizar el recuperatorio de los entregables que consiste en una parte práctica para resolver en 1 hora y una parte teórica para responder oralmente.

:Examen final: 
	- Se puede presentar un proyecto integrador individual con Simulink y/o Python.
	- También se puede rendir mediante la resolución de un ejercicio con Python para resolver en 1 hora y una parte teórica para responder oralmente.


Instalación de herramientas
===========================

:Python: 
	- Descargamos e instalamos `Python 3.8.10 <https://www.python.org/downloads/release/python-3810/>`_ 
	- Elegir instalador para Windows 64 bits (archivo python-3.8.10-amd64.exe)
	- Realizamos una instalación customizada (Install for all users - Create shortcuts for installed applications - Add Python to environment variables - Precompile standard library - pip - C:\Program Files\Python38) 
	- Verificamos la instalación de Python ejecutando desde consola ``python --version``
	- Verificamos la instalación de PIP ejecutando desde consola ``python -m pip --version``

:OBS Studio: 
	- Descargar instalador desde la `Página de descarga <https://obsproject.com/es>`_ e instalar

:Blender: 
	- Descargar instalador desde la `Página de descarga <https://www.blender.org/>`_ 
	- Es una herramienta para modelado 3D, animación, edición de video, ...	


Creación de entorno virtual
===========================

.. code-block:: console 

	pip install virtualenv  #

	Podemos ver todo lo que está instalado con pip en el sistema:

	pip freeze  # Muestra el listado de paquetes instalados

	Ahora creamos el entorno virtual, el cual debe estar en un directorio particular
	Creamos la siguiente carpeta para el proyecto mano

	C:\Cosas\2021\Almeria\mano\EntornoVirtual

	cd C:\Cosas\2021\Almeria\mano\EntornoVirtual

	virtualenv mano

	Demos ahora activar este entorno virtual

	.\mano\Scripts\activate

	Podemos ver que en el entorno virtual tenemos el python pero ningún paqueta instalado

	pip install numpy
	pip install matplotlib

	Descativamos el entorno virtual con

	deactivate

	Para borrar el entorno virtual hay que borrar la carpeta donde se creó



Entregable Clase 01
===================

- Punto de partida: Computadora sin Python instalado
- Se pide explicar (en video o durante la clase) la manera en que se instala Python y se crea un entorno virtual.
- Este primer entregable tiene como objetivo poner a punto el mecanismo de entrega de los ejercicios de cada clase.

		
Introducción
============

- Brindar al estudiante herramientas de programación de microcontroladores para el procesamiento digital de señales.
- Conocimientos sobre programación de hardware específico para tratamiento de señales.
- Complementa lo desarrollado en "Teoría de Señales y Sistemas Lineales" y "Tratamiento Digital de Señales". 


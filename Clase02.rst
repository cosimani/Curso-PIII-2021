.. -*- coding: utf-8 -*-

.. _rcs_subversion:

Clase 02 - PIII 2021
====================
(Fecha: 13 de agosto)


Herramienta de edición de texto y código fuente
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Descargar `Sublime Text <https://www.sublimetext.com>`_



Instrucciones básicas de Python
===============================

**Captura de Datos:** *input*

**Muestra de Datos:** *print*

.. code-block:: python 

	# Se pide el ingreso de un número por teclado y se muestra el número y el tipo de dato.
	# Si no forzamos el tipo de dato en el ingreso, lo toma como string (cadena de caracteres)
	numero = input( 'Escriba un número: ' )
	print( 'El número ingresado es: ', numero )
	print( 'El tipo del dato ingresado es ', type( numero ) )


¿Cómo ejecutamos este código?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Creamos una carpeta para almacenar nuestros códigos, por ejemplo: C:\\Cosas\\2021\\PIII2021\\Codigos\\Clase02
- Abrimos Sublime Text y guardamos estas líneas de código en un archivo llamado ``primerCodigo.py``
- Abrir consola con CMD
- Entrar al entorno virtual creado en la primer clase, ejecutando lo siguiente (acomodar la ruta de ser necesario):

.. code-block:: bash 

	cd C:\Cosas\2021\PIII2021\EntornosVirtuales  # Accedemos a la carpeta

	.\entorno01\Scripts\activate  # Activamos el entorno virtual

	pip install numpy==1.19.5  # Instalamos numpy en la versión 1.19.5

	# Si aparece un mensaje Warning diciendo que hay una versión nueva de pip, podemos ejecutar el comando que nos recomienda

	pip freeze  # Revisamos el listado de paquetes instalados en el entorno virtual

	python C:\Cosas\2021\PIII2021\Codigos\Clase02\primerCodigo.py

	# Recordar que para salir debemos desactivar el entorno virtual
	deactivate

	exit  # Para cerrar la consola


Entregable Clase 02
===================

- Punto de partida: Computadora sin Python instalado
- Se pide explicar (en video o durante la clase) la manera en que se instala Python y se crea un entorno virtual.
- Este primer entregable tiene como objetivo poner a punto el mecanismo de entrega de los ejercicios de cada clase.

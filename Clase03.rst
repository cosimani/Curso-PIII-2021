.. -*- coding: utf-8 -*-

.. _rcs_subversion:

Clase 03 - PIII 2021
====================
(Fecha: 18 de agosto)


IDE para Python
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

- Descargar `Spyder <https://www.spyder-ide.org/>`_
- Versión actual: 5.1.1
- Instalar para todos los usuarios.


Módulos y paquetes
==================

**Módulo**: Es un archivo Python cuyas utilizadades (funciones, clases, etc.) se pueden usar desde otro archivo.

- Supongamos el archivo ``matematicas.py``

.. code-block:: python 

	def sumar( a, b ) :
	    return a + b

	def restar( a, b ) :
	    return a - b

- Podremos utilizar estas funciones de la siguiente manera:

.. code-block:: python

	import matematicas  # Esta línea importa todos los recursos del archivo matematicas.py

	print( matematicas.sumar( 7, 5 ) )
	print( matematicas.restar( 17, 15 ) )

- Si sólo deseamos importar la función ``sumar`` hacemos:

.. code-block:: python

	from matematicas import sumar

	print( sumar( 7, 5 ) )

- Otras alternativas:

.. code-block:: python
	
	from matematicas import sumar, restar

	from matematicas import *


**Paquetes**: Es una carpeta que contiene varios módulos. 

.. code-block:: bash 

	operaciones/
	    |-- __init__.py    # Este archivo indica que la carpeta operaciones es un paquete y no una simple carpeta 
	    |-- matematicas.py
	    |-- matrices.py


- Alternativas para importar

.. code-block:: python
	
	import operaciones.matematicas

	from operaciones import matematicas

	from operaciones.matematicas import sumar




Entregable Clase 03
===================

- Punto de partida: Entorno virtual creado y usando Sublime Text para escribir el código desde cero
- Asigne el valor 7 a la variable  x .
- Verifique e imprima la veracidad de la siguiente afirmación: ``x**2 + 5 − 2`` igual a ``( x ∗ 5 − 9 ) ∗ 2`` 
- Verifique e imprima que no es cierto si x es -7


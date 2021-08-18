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

**Módulo**: Es un archivo Python cuyas utilidades (funciones, clases, etc.) se pueden usar desde otro archivo.

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


Biblioteca numpy
================

- Vectores, matrices, gran colección de funciones matemáticas.
- `Documentación de numpy <https://numpy.org/doc/stable/index.html>`_ 


**Algunos ejemplos de su uso**

.. code-block:: python

	import numpy as np

	lista = [ 25., 8., 20., 75. ] 
	print( type( lista ), lista )

	v = np.array( lista )  # Transformo la lista en vector
	print( '\nv =', v )  # El vector no lleva comas separando los elementos
	print( 'tipo de v:', type( v ) )  # el tipo es numpy.ndarray
	print( 'longitud de v:', len( v ) )

	# máximo y mínimo valor de v
	print( 'máximo de v:', v.max(), 'o', np.max( v ) )  # función de numpy.ndarray: np.max()
	print( 'mínimo de v:', v.min(), 'o', np.min( v ) )


.. code-block:: python

	import numpy as np
	u = np.array( [ 5, 9, 10, -1 ] )  # Transforma la lista en vector

	v = np.array( [ -2, 0, 5, 4 ] )

	print( "vector u =", u )
	print( "vector v =", v )

	z = u + v 
	print( "z = u + v  ->  z =", z )

	w = 2 * z
	print( "2 * z =", w )

	t = w - 3
	print( "Restamos 3 a cada elemento del vector anterior", t )



Entregable Clase 03
===================

- Punto de partida: Entorno virtual creado y usando Sublime Text para escribir el código desde cero
- Asigne el valor 7 a la variable  x .
- Verifique e imprima la veracidad de la siguiente afirmación: ``x**2 + 5 − 2`` igual a ``( x ∗ 5 − 9 ) ∗ 2`` 
- Verifique e imprima que no es cierto si x es -7


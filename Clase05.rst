.. -*- coding: utf-8 -*-

.. _rcs_subversion:

Clase 05 - PIII 2021
====================
(Fecha: 24 de agosto)

Cuadernos de código y herramientas
==================================

- Jupyter Notebook
- Anaconda
- Google Colab

.. figure:: images/clase05_jupyter_ana_colab.png



`Iteraciones y decisiones (ipynb) <https://colab.research.google.com/drive/1u-X1uIGoHCKf_QRb1jTdBZ_Ap_Z7hhYq?usp=sharing>`_ 
================================


**Sentencia if**

.. code-block:: python

	edad = int( input( 'Ingrese edad: ' ) )

	if edad < 0 :
	    print( 'Error' )
	elif edad < 18 :
	    print( 'Menor de edad' )
	else :
	    print( 'Mayor de edad' )

	# Operadores para comparar: ==  !=  <  >  <=  >=

**Sentencia for**

.. code-block:: python

	suma = 0
	mis_numeros = [ 4, 8, 12, 18 ] 

	# la variable numero designará a los elementos de la lista
	for numero in mis_numeros :
	    suma = suma + numero
	    print( 'Esto se imprime en cada ciclo. Suma parcial =', suma )

	print( 'Esto se imprime fuera del ciclo' )
	print( 'La lista es:', mis_numeros )
	print( 'La suma de los números de la lista es:', suma )


	print( '\nUn for para range de 0 a 3' )
	for i in range( 4 ) :
    	print( i )

    imagenes = [ 'impulso.jpg', 'gráficos.png', 'esquema.jpg' ]
	for imagen in imagenes :
	    print ( '\nEl nombre de la imagen es: {0} y el largo ' \
	            'del nombre es: {1}'.format( imagen, len( imagen ) ) )    

	mi_lista = [ 'manzana', 'bananas', 'uvas', 'peras' ]
	# La primera variable (c en nuestro caso) es el contador
	# La segunda variable (valor en nuestro caso) es precisamente el valor almacenado en cada posición
	# El segundo parámetro de eumerate es desde dónde comienza la enumeración 
	for c, valor in enumerate( mi_lista, 0 ) :
	    print( '\n', c, valor )

**Sentencia while**

.. code-block:: python

	n = 5
	print( 'Loop 1 started.' )
	while n > 0 :
	    n -= 1
	    if n == 2 :
	        break
	    print( n )
	print( 'Loop 1 ended.' )

	n = 5
	print( 'Loop 2 started.' )
	while n > 0 :
	    n -= 1
	    if n == 2 :
	        continue
	    print( n )
	print( 'Loop 2 ended.' )


`Sonidos humanamente audibles (ipynb) <https://colab.research.google.com/drive/1CZ_HpWmftsejvJAuUKM54AiCrQVE1km-?usp=sharing>`_ 
=====================================

- Aproximadamente entre 20 Hz y 20 kHz

Entregable Clase 05
===================

- Punto de partida: Cuaderno Colab llamado clase05_entregable05.ipynb
- Reproducir la escala pentatónica menor de La
- Buscar información donde desee.
- Deben sonar las notas que se pueden escuchar `Aquí <https://es.wikipedia.org/wiki/Archivo:PentMinor.mid>`_ 
- Entrar al siguiente `link para ver el registro de los entregables <https://docs.google.com/spreadsheets/d/1Qpp9mmUwuIUEbvrd_oqsQGuPOO9i1YPlHa_wBWTS6co/edit?usp=sharing>`_ 
- En caso de compartir video, se realiza en Youtube (No listado) compartiendo con el docente por mensaje privado de Teams.
- `Mesas de trabajo en Discord <https://discord.gg/TFKzMXrNCV>`_ 


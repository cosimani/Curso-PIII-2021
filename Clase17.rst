.. -*- coding: utf-8 -*-

.. _rcs_subversion:

Clase 17 - PIII 2021
====================
(Fecha: 18 de octubre)

Creación de GUI
===============

- QtDesigner para diseñar una interfaz con modalidad Drag and Drop.
- Creación de entorno virtual
- Instalación de bibliotecas
- Características de la biblioteca Qt
- Manejo de eventos
- Gráficos y reproducción

**Información**

- Ir a https://www.qt.io/download para descargar el QtCreator. No hace falta más que el QtCreator que tiene el QtDesigner que nos genera el .ui
- Ver aquí cómo se utiliza el .ui para generar la interfaz. https://www.pythonguis.com/tutorials/pyside-first-steps-qt-designer/


.. code-block:: bash 

	cd C:\Cosas\2021\EntornosVirtuales
	mkdir PIII_con_GUI
	cd PIII_con_GUI

	virtualenv entorno_gui_piii
	.\entorno_gui_piii\Scripts\activate

	pip install numpy==1.19.5
	pip install shiboken6==6.0.0
	pip install PySide6==6.0.0 
	pip install matplotlib==3.3.4 
	pip install scipy==1.7.1
	pip install sounddevice==0.4.2

	python C:\Cosas\2021\PIII2021\Codigos\Clase17\ventana.py



Entregable Clase 17
===================

- Punto de partida: Programa realizado por el docente.
- Agregar las funciones de generación de tonos y graficar la suma de varios tonos y reproducirlos.
- Reestructurar el layout de la interfaz.
- Entrar al siguiente `link para ver el registro de los entregables <https://docs.google.com/spreadsheets/d/1Qpp9mmUwuIUEbvrd_oqsQGuPOO9i1YPlHa_wBWTS6co/edit?usp=sharing>`_ 
- El link de Youtube se comparte con el docente por mensaje privado de Teams.



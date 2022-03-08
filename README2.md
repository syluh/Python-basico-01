<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Knowledge-Based-Systems/Python-basico-01">
    <img src="images/logo-kbs.png" alt="logo-kbs" width="80" height="80">
  </a>

<h3 align="center">Python-basico-01</h3>

  <p align="center">
    Primeros pasos en Python
    <br />
    <br />
    <br />
   
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#Git-y-GitHub">Git y GitHub</a>
    </li>
    <li><a href="#Instalación-de-Python">Instalación de Python</a></li>
    <li><a href="#Librerías-en-Python">Librerías en Python</a></li>
    <li><a href="#Ejemplos-básicos-Python">Ejemplos-Básicos-Python</a></li>
    <li><a href="#Ejemplos-con-Pandas">Ejemplos con Pandas</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## Git y GitHub


[Conceptos y comandos de Git y GitGub](https://www.canva.com/design/DAEtXTH2Kg8/qwC_wkqstmOwShmmnFFdEw/view?website#2) 

* Comandos globales de GIT antes de empezar a trabajar (una sola vez):
```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```
* Comandos básicos de GIT
```sh
git clone 	# [dirección del repositorio]
git add .   # agregar archivos al repositorio
git commit  -a -m"mensaje"    # poner archivos en proceso de versionamiento en el local
git push # subir los cambios al servidor
git status  # ver estado de los archivos
git pull # [actualizar cambios que está en el servidor]
```

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Instalación de Python

1. Descargar de la página oficial: [https://www.python.org/](https://www.python.org/) 
2. Revisar el siguiente enlace: [Python](https://www.canva.com/design/DAE6ZNEML6k/ZMXgexKAXGd-O3giMJVHjQ/view?website#2) 


## Librerías en Python

Uso de entornos virtuales: [Entornos-Python](https://www.canva.com/design/DAE6ZGmZvUo/-onO254gacXbtn5caOwN4g/view?website#2) 

* Primer parte
1. 
```sh
   pip install virtualenv
```
2. Crear entorno virtual
```sh
virtualenv ruta/carpeta/entorno
```
3. Activar entorno en Linux
```sh
source ruta-a-carpeta-entorno/bin/activate
```
4. Activar entorno en Windows
```sh
\ruta-a-carpeta-entorno\Scripts\activate.bat
```

* Segundo Parte
1. Instalar paquetes en Python 
```sh
   pip install jupyter
   pip install jupyterlab
   pip install pandas
```

<p align="right">(<a href="#top">back to top</a>)</p>

## Ejemplos-Básicos-Python

Usted puede ejecutar los siguiente ejemplos, ingresando a la carpeta **ejemplos-python-basicos**. En la carpeta, a través del terminal, digitar
```python
jupyter notebook
```

* Ejemplo 01 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-basicos/Ejemplo01.ipynb) 
```python
# cadena - str
mensaje = "hola mundo"
print(mensaje)
print("%s" % (mensaje))
print(f"{mensaje}")
```

* Ejemplo 02 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-basicos/Ejemplo02.ipynb) 
```python
nombre = input("Ingrese nombre del persona: ")

edad = int(input("Ingrese edad de persona: "))

sueldo = float(input("Ingrese el sueldo de la persona: "))
                    
mensajeFinal = "Nombre:%s\nEdad:%d\nSueldo:%.2f\n" % (nombre, 
        edad, sueldo)

print(mensajeFinal)
```

* Ejemplo 03 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-basicos/Ejemplo03.ipynb) 
```python
sueldo = 110

while sueldo <= 120:
    print(f"{sueldo}")
    sueldo = sueldo + 5

print("%.2f" % sueldo)
```

* Ejemplo 04 
```python
sueldo = 110

for i in range(0, sueldo):
    print(i)

sueldo = 110

for i in range(0, sueldo, 20):
    print(i)
```

* Ejemplo 05 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-basicos/Ejemplo05.ipynb) 
```python
lista1 = []

lista2 = ["a", 1, [], "b"]

lista3 = [1]
lista3.append("b")
lista3.append("c")
lista3.append(10)



for i in lista2:
    print(i)
```
<!-- USAGE EXAMPLES -->
## Ejemplos con Pandas

Usted puede ejecutar los siguiente ejemplos, ingresando a la carpeta **ejemplos-python-pandas**. En la carpeta, a través del terminal, digitar
```python
jupyter notebook
```

* Ejemplo-Pandas-01 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-pandas/Ejemplo-Pandas-01.ipynb) 
```python
import pandas as pd

mi_df = pd.DataFrame(({'a': [11,12,13], 'b': [21,22,23]}))
print(mi_df)

data = {'ciudad': ['Loja', 'Pichincha', 'Guayas'],
        'capital' : ['Loja', 'Quito', 'Guayaquil'],
        'zona'  : [7, 8, 1]}
frame = pd.DataFrame(data) # Creando un DataFrame desde un diccionario
frame
```

* Ejemplo-Pandas-02 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-pandas/Ejemplo2-Pandas-02.ipynb) 
```python
import pandas as pd
df = pd.read_csv("data/Matrimonios_2014.csv")
df.keys()

df.mes_insc.value_counts()[:12].sort_values(inplace=False).plot(kind='barh')
```

* Ejemplo-Pandas-03 - [codigo](https://github.com/Knowledge-Based-Systems/Python-basico-01/blob/main/ejemplos-python-pandas/Ejemplo-Pandas-03-BD.ipynb) 
```python
import pandas as pd
import sqlite3

connection = sqlite3.connect("data/instituciones.db")
connection.text_factory = str
result = pd.read_sql_query("SELECT * from educativas", connection)
```


<p align="right">(<a href="#top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

René Elizalde - [@reroes](https://twitter.com/reroes) - rrelizalde@utpl.edu.ec


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

[https://investigacion.utpl.edu.ec/es/grupos/kbs](https://investigacion.utpl.edu.ec/es/grupos/kbs) 
<p align="right">(<a href="#top">back to top</a>)</p>


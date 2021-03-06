# PROYECTO 1 G-8 TYTYSDB
TytusDB is an Open Source Database Management System
## Integrantes 
* Julio Roberto Garcia Escalante 201503922
* Edgar Rolando Herrera Rivas 201520498
* Ricardo Humberto Fuentes Garcia 201513747
* Christian Enrique Ramos Alvarez 201504444
### Descripcion del proyecto 
Este sistema de administracion de datos, esta estructurado de la siguiente manera 
* **Servidor:** Este servidor esta hecho en lenguaje de python que utiliza la herramienta flask para poder realizar dicho servidor 
* **Cliente** 
Esta hecho en python con ayuda de angular Cli para la interfaz grafica ya que el grupo considero que angular tienen 
muy buenas heramientas que son amigables con el usuario 
### **Herramientas a utilizar**
* Python
* Flask
* Angular
* PostMan
#### Python:  es un lenguaje de programación interpretado cuya filosofía hace hincapié en la legibilidad de su código. 
Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, 
en menor medida, programación funcional
#### Flash: Es un framework minimalista escrito en Python que permite crear aplicaciones web rápidamente y con un mínimo número de líneas de código. 
Está basado en la especificación WSGI de Werkzeug y el motor de templates Jinja2 y tiene una licencia BSD.
#### Angular: Es un framework para aplicaciones web desarrollado en TypeScript, 
de código abierto, mantenido por Google, que se utiliza para crear y mantener aplicaciones web de una sola página.
# Manual de Tecnico
## Servidor 
### Intalacion Sistema operativo Linux 
**Python3** 
* Paso 1: Se acualizan los repositorios 
```linux 
sudo apt update
```
* Paso 2: Se procede a intallar Python 3 
```linux 
sudo apt install python3.8
```
* Paso 3: Verificamos que la instalacion este correcta 
```linux 
python ––version
```
* Paso 4: Se vuelve actualizar los repositorios 
```linux 
sudo apt update
```

**Flask**
* Paso 1: Para la instalacion de Flask es necesario ya tener PIP3 en el ordenador, luego se coloca este comando para poder hacer la instalacion de flask 
```linux 
pip install Flask
```
**Angular**
* Paso 1: Se acualizan los repositorios 
```linux 
sudo apt update
```
* Paso 2: Es necesario tener en cuenta que para la instalacion de Angular Cli se necesita tener instalado instalar NodeJs y Node Package Manager (NPM).
    * Paso 2.1 Instalacion de Node JS 
    ```linux
    curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
    sudo apt-get install -y nodejs
    ```
    * Paso 2.2 Instalacion de NPM:
    ```linux
    sudo npm install npm@latest -g
    ```

* Paso 3: Instalacion de Angular CLI 
```linux
sudo npm install -g @angular/cli
```



### Codigo Servidor 
Paso 1: Se agregan las librerias de Flask, request para poder realizar el servidor WEB
```python
from flask import Flask, request
```
Paso 2: Se inicializa Flask para poder manejar una variable global 
```python
app = Flask(__name__)
```
Paso 3: Se realiza los metodos para las peticiones ya sea de tipo POST, GET
```python
@app.route('/prueba',methods = ['GET'])
def prueba():
    return 'prueba'
```
Paso 4: Se Levanta el servidor
```python
python3 Servidor_flask.py 
```
Paso 5: Se realiza las pruebas en la Herramienta Postman para verificar que el servidor no tenga ningun error.




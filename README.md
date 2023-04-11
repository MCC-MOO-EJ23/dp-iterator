# Iterator - Caso práctico

### Intención

Provee una manera de acceder secuencialmente a los elementos de un objeto agregado sin exponer su representación subyacente.

### Clasificación

Patrón de Comportamiento

### Vista Estructural

![image](https://user-images.githubusercontent.com/84739791/231038297-e955d5cd-b811-41d5-bfe8-24ded9025b70.png)

### Vista Dinámica

![image](https://user-images.githubusercontent.com/84739791/231038378-2564b637-67c5-4a69-84ac-fdaf94c15276.png)

### Ejemplo Real

Actualmente estamos desarrollando un programa que recibe una estructura de 
Empleados, estos empleados tiene a su vez cero o muchos subordinados, el 
problema que tenemos es que es necesario obtener todos los empleados de la 
estructura.
Internamente, la estructura de datos es un Árbol en donde la raíz es el CEO y las 
ramas son los empleados de más bajo rango, el orden con el cual hay que recorrer 
los empleados no es muy importante pero sí que recorramos todos.
De entrada tenemos que la estructura de datos interna es un Árbol y esto podría 
hacer que batallemos a la hora de recorrerlo ya que necesitaremos algún
procedimiento recursivo que nos asegure el recorrido completo del Árbol. Otro 
problema podría ser si cambiará la estructura de datos a otro tipo, esto provocaría
que nuestro programa deje de funcionar.

![image](https://user-images.githubusercontent.com/84739791/231038592-a2036655-1cbe-4bd1-8f51-07705f1f5479.png)


### Solución con el patrón Iterator:

La idea consiste en hacer que nuestra clase (que contiene la estructura de datos)
nos proporcione una operación con la que podremos crear un Iterador, este 
iterador deberá seguir una interface que defina los métodos mínimos hasNext y 
next que nos servirán para validar que existan más elementos en la estructura y 
el otro para obtener el elemento siguiente respectivamente.

![image](https://user-images.githubusercontent.com/84739791/231038843-aca49053-7bbb-43a6-b7e8-e71be3f120a8.png)

![image](https://user-images.githubusercontent.com/84739791/231038966-5e653dc5-8126-4064-b70e-146c8bcad2e7.png)

# Ejecutar Java-App 

* Cargue las Extensiones Java de VS Code correcta y completamente.
* En la clase principal de clic sobre el botón Play.


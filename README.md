# 馃摑 Contact Diary Application 

##  馃幆 Descripci贸n 

El gestionar los contactos del d铆a a d铆a puede ser un trabajo a veces complicado y engorroso. Por ende, una soluci贸n 
贸ptima es el uso de Software que ayude a que las tareas organizativas y de consultas de los contactos sea de la 
manera m谩s sencilla y r谩pida. **Contact Diary Application** es una soluci贸n que permite desarrollar las actividades
mencionadas; caracterizandose su dise帽o y tu interfaz sencilla de usar, permitiendo que el usuario pueda efectuar
las operaciones de listado, guardado, borrado y actualizado de su agenda de contactos. 

## 馃搵 Tabla de Contenido 

1. 驴C贸mo instalar Contact Diary Application?
2. 驴C贸mo correr Contact Diary Application? 
3. Comprensi贸n de Conceptos B谩sicos 

## 馃斀 驴C贸mo instalar Contact Diary Application?

> *Contact Diary Application fue creado con el uso del lenguaje de programaci贸n **PHP**, en su versi贸n **8.1.2**, lo cual
debe de considerarse para que la herramienta funcione correctamente.*

Pre-Requisitos:

1. Instalar PHP versi贸n 8 o superior. 
2. Instalar [XAMPP](https://www.apachefriends.org/).  


Si se encuentra en un entorno **Linux** ejecute los siguientes comandos: 

    sudo apt update 
    sudo apt install php8.1

## 鈿? 驴C贸mo correr Contact Diary Application? 

Inicie el lanzador de **XAMPP** para correr el servidor **Apache** y el motor de base de datos **SQL**:

    sudo /opt/lampp/manager-linux-x64.run

Posteriormente, cree la base de datos en su entorno de preferencia SQL (**Se recomienda Phpmyadmin**)
utilizando el script encontrado **/database/scrip.sql** del proyecto. :

    http://127.0.0.1/phpmyadmin

Posteriormente, ejecute en su navegador de preferencia el siguiente comando: 
    
    http://localhost/contactDiaryApplication/index.php

## 馃摎 Comprensi贸n de Conceptos B谩sicos 
### 1. 驴Cu谩ndo se utiliza el m茅todo OPTIONS en las peticiones HTTP? 

Es implementado cuando se desea saber informaci贸n adicional sobre las opciones de comunicaci贸n hacia un destino, este puede ser un servidor web. Adem谩s, permite que puedan consultarse aspectos como los m茅todos HTTP (POST, GET, PUT, DELETE) permitidos por un servidor a trav茅s del acceso por un nombre de dominio y dem谩s capacidades que contenga el mismo.

### 2. Menciones por lo menos 3 tipos de c贸digos HTTP que existen 

1. **200 OK**: Es un c贸digo que informa que la solicitud al servidor se ejecuto de manera exitosa.
2. **404 (NOT FOUND)**: Especifica que el servidor no pudo encontrar el recurso deseado.
3. **500 (Internal Server Error)**: Ocurre cuando se presenta un error en el servidor que no se ha podido gestionar.

### 3. 驴Es 贸ptimo manejar sesiones en una API REST?, explique el por qu茅 y de un ejemplo

Si, ya que la arquitectura REST le permite al usuario interactuar con el servidor de manera eficiente en cuanto a sus necesidades (M茅todos HTTP) y este tambi茅n permite distintos tipos de autenticaci贸n por los encabezados HTTP, como lo es el caso de la b谩sica; o bien por Token, permitiendo que el servidor genere un registro en base de datos de acuerdo a  las credenciales del usuario, para as铆 evitar que tenga que solicitarse nuevamente sus datos.

Un ejemplo pr谩ctico es cuando deseamos entrar a un login de una p谩gina, estos datos bien son enviados a trav茅s del m茅todo POST, de forma segura, sin ser visualizados por la URL del navegador, y bien el servidor efectua el tipo de autenticaci贸n que tenga configurada (B谩sica, por token, etc).

### 4. 驴Qu茅 valor imprime el siguiente c贸digo (Case 1) ? 

    Question 4
    $a = array("A", "B", 1 => "C", "D", 2 => "E"); 
    echo count($a);
    Answer: Return 3 
    Array 3 postions ["A", "C", "E"];
    echo $a[0];
    echo $a[1];
    echo $a[2];

### 5. 驴Qu茅 valor imprime el siguiente c贸digo (Case 2)? 

    Question 5 
    $a=1;
    ++$a;
    $a *= $a;
    echo $a--;  
    Return 4, then decrement $a to 3

漏 2022 Hecho con 鉂わ笍 por Ysnaldo Jos茅 L贸pez

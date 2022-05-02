nodejs-mysql-jwt-autenticación
Regístrese/Inicie sesión con Node.js, MySql y JWT (JSON Web Token).

Requisitos previos del software:

Nodo.js
Joi
mysql
Token web JSON
Nodemailer
Pavonearse
Instalación
Este es un módulo de Node.js disponible a través del registro npm .

Antes de instalar, descargue e instale Node.js. Se requiere Node.js 0.10 o superior.

Si se trata de un proyecto nuevo, asegúrese de crear uno package.jsonprimero con el npm initcomando .

La instalación se realiza mediante el npm installcomando :

$ npm install express

Inicio rápido
La forma más rápida de comenzar con Express es utilizar el ejecutable express(1)para generar una aplicación como se muestra a continuación:

Instala el ejecutable. La versión principal del ejecutable coincidirá con la de Express:

$ npm install -g express-generator@4

Create the app:

$ express nodejs-mysql-jwt-authentication && cd nodejs-mysql-jwt-authentication

Install dependencies:

$ npm install

Start the server:

$ npm start

Ver el sitio en: http://localhost:3000

Joi

Joi es un lenguaje de descripción de esquemas de objetos y un validador para objetos de JavaScript. Joi le permite crear planos o esquemas para objetos de JavaScript para garantizar la validación de la información clave. Para comenzar con joi, primero debe instalarlo y agregarlo como una dependencia a su proyecto:

La instalación se realiza mediante el comando npm install:

$ npm install @hapi/joi

extensiones joi-date para reglas de fecha avanzada.

$ npm install @hapi/joi-date

MySql

Este es un controlador de node.js para mysql .

La instalación se realiza mediante el comando npm install:

$ npm install mysql

Token web JSON | JWT

JSON Web Token es un formato de representación de reclamos compacto destinado a entornos con limitaciones de espacio, como encabezados de autorización HTTP y parámetros de consulta de URI. Un token web JSON (JWT) es un objeto JSON que se utiliza para transferir información de forma segura a través de la web (entre dos partes).

$ npm install jsonwebtoken

Swagger

El módulo Swagger UI Express le permite servir documentos API generados automáticamente por swagger-ui desde express, basados ​​en un archivo swagger.json. El resultado es una documentación viva para su API alojada desde su servidor de API a través de una ruta.

$ npm install swagger-ui-express swagger-jsdoc

NodeMailer

es un módulo para aplicaciones Node.js que permite enviar correos electrónicos de forma sencilla. Enviar correo a través de Gmail

$ npm install nodemailer

Creación de base de datos y tabla.

create database TEST;

use TEST;

create table users(
    userId int primary key auto_increment,
    email varchar(30) unique,
    password varchar(250),
    displayName varchar(50),
    phoneNumber bigint
);
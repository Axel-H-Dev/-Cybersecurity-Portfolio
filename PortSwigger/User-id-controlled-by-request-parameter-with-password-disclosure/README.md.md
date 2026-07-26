# User ID Controlled by Request Parameter with Password Disclosure

## 📌 Descripción
Este laboratorio demuestra una vulnerabilidad **IDOR (Insecure Direct Object Reference)** donde la aplicación utiliza un parámetro controlado por el usuario para acceder a información sensible. Debido a una validación insuficiente, es posible visualizar datos de otra cuenta, incluyendo su contraseña.

## 🎯 Objetivo
Acceder a la información de otro usuario modificando un parámetro de la petición HTTP y utilizar las credenciales expuestas para completar el laboratorio.

## 🔍 Vulnerabilidad
- Broken Access Control
- Insecure Direct Object Reference (IDOR)
- Password Disclosure

## 🛠️ Herramientas
- Burp Suite Community Edition
- Navegador Web

## 🚀 Procedimiento
1. Iniciar sesión con un usuario válido.
2. Interceptar la petición hacia `/my-account`.
3. Modificar el parámetro `id` por el de otro usuario.
4. Analizar la respuesta del servidor.
5. Identificar la contraseña expuesta y acceder con esa cuenta.

## 🚨 Impacto
La exposición de credenciales permite la toma de control de cuentas y el acceso no autorizado a información sensible.

## 🛡️ Mitigación
- Validar autorizaciones en el servidor.
- No exponer contraseñas en respuestas.
- Aplicar el principio de mínimo privilegio.

## 📚 Lecciones aprendidas
- Manipulación de parámetros HTTP.
- Identificación de vulnerabilidades IDOR.
- Importancia del control de acceso del lado del servidor.

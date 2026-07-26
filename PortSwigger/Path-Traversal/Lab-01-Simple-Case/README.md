# Lab 01 - File Path Traversal

## Objetivo

Comprender cómo una aplicación puede acceder a archivos fuera del directorio permitido.

---

## Conceptos

- HTTP GET
- Query Parameters
- filename
- Burp Suite
- HTTP History
- Path Traversal
- Linux File System

---

## Lo que aprendí

Aprendí a utilizar Burp Suite para localizar la petición HTTP que obtiene una imagen.

Entendí que el parámetro `filename` representa el archivo solicitado por el servidor.

También comprendí cómo un servidor vulnerable puede interpretar rutas fuera del directorio esperado cuando no valida correctamente la entrada del usuario.

---

## Herramientas

- Burp Suite Community
- PortSwigger Academy

---

## Dificultad

⭐⭐☆☆☆

---

## Tiempo

1 hora 15 minutos

---

## Reflexión

Fue mi primer laboratorio utilizando Burp Suite.

La mayor dificultad fue aprender a identificar la petición correcta dentro del HTTP History.

Una vez entendido ese proceso, el laboratorio tuvo mucho más sentido.
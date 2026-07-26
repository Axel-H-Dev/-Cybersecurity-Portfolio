# Username Enumeration via Different Responses

## 📌 Descripción
Este laboratorio muestra cómo pequeñas diferencias en las respuestas del servidor permiten descubrir usuarios válidos antes de realizar un ataque de fuerza bruta.

## 🎯 Objetivo
Identificar un usuario válido mediante Burp Intruder y posteriormente descubrir su contraseña.

## 🔍 Vulnerabilidad
- Username Enumeration
- Information Disclosure

## 🛠️ Herramientas
- Burp Suite Community Edition
- Burp Intruder

## 🚀 Procedimiento
1. Interceptar la petición de login.
2. Enviar la solicitud a Intruder.
3. Configurar un ataque **Sniper**.
4. Cargar una lista de usuarios.
5. Comparar **Status Code**, **Length** y contenido de las respuestas.
6. Identificar el usuario válido.
7. Repetir el proceso con una lista de contraseñas.

## 🚨 Impacto
La enumeración de usuarios facilita ataques de fuerza bruta y credential stuffing.

## 🛡️ Mitigación
- Utilizar mensajes de error genéricos.
- Igualar tiempos y tamaños de respuesta.
- Implementar Rate Limiting y MFA.

## 📚 Lecciones aprendidas
- Uso de Burp Intruder.
- Payloads.
- Interpretación de Status Code y Response Length.
- Enumeración de usuarios.

# Lab: User ID controlled by request parameter with unpredictable user IDs

## Información del laboratorio

-   **Categoría:** Access Control
-   **Plataforma:** PortSwigger Web Security Academy
-   **Estado:** ✅ Resuelto

## Objetivo

Analizar una aplicación web para determinar si es posible acceder al
perfil de otro usuario manipulando el identificador enviado en la
solicitud.

## Vulnerabilidad

La aplicación utilizaba identificadores de usuario impredecibles (UUID).
Sin embargo, el servidor no verificaba correctamente que el recurso
solicitado perteneciera al usuario autenticado.

Como resultado, era posible modificar el parámetro correspondiente al
identificador y acceder a la información de otro usuario.

## Pasos realizados

1.  Iniciar sesión con un usuario válido.
2.  Analizar las solicitudes utilizando Burp Suite.
3.  Identificar el parámetro que contenía el User ID.
4.  Obtener el identificador de otro usuario disponible en la
    aplicación.
5.  Reemplazar el valor del parámetro.
6.  Confirmar que la aplicación mostraba información perteneciente a
    otro usuario.

## Impacto

Esta vulnerabilidad permite el acceso no autorizado a información de
otros usuarios, comprometiendo la confidencialidad de los datos.

## Mitigación

-   Validar la autorización en el servidor para cada solicitud.
-   Verificar que el recurso solicitado pertenezca al usuario
    autenticado.
-   No confiar únicamente en identificadores impredecibles como
    mecanismo de seguridad.

## Herramientas utilizadas

-   Burp Suite
-   Navegador web
-   PortSwigger Web Security Academy

## Aprendizaje

Este laboratorio demuestra que utilizar UUID u otros identificadores
difíciles de adivinar **no reemplaza un control de autorización
adecuado**. La autorización siempre debe verificarse en el servidor
antes de entregar cualquier recurso.

------------------------------------------------------------------------

**Estado final:** Laboratorio completado exitosamente.

# 2FA Simple Bypass

## 📌 Descripción
Este laboratorio demuestra un fallo lógico donde la aplicación no verifica correctamente que el proceso de autenticación multifactor haya finalizado antes de conceder acceso.

## 🎯 Objetivo
Acceder a una cuenta omitiendo la verificación del segundo factor de autenticación.

## 🔍 Vulnerabilidad
- Broken Authentication
- Multi-Factor Authentication Bypass

## 🛠️ Herramientas
- Burp Suite
- Navegador Web

## 🚀 Procedimiento
1. Iniciar sesión con credenciales válidas.
2. Analizar el flujo de autenticación.
3. Acceder directamente al recurso protegido sin completar el 2FA.
4. Verificar el acceso concedido.

## 🚨 Impacto
Un atacante con credenciales válidas puede eludir el segundo factor y comprometer la cuenta.

## 🛡️ Mitigación
- Validar el estado del 2FA en cada recurso protegido.
- No crear una sesión completamente autenticada hasta finalizar el MFA.
- Revisar la lógica de autorización.

## 📚 Lecciones aprendidas
- Funcionamiento del MFA.
- Identificación de fallos lógicos.
- Análisis del flujo de autenticación.

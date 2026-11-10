<div align="center">

# Edupe

**Asistencia y gestión diaria para instituciones educativas del Perú**

Marcación QR · Control de jornada · Reportes · Agenda de dirección

[![Estado del proyecto: En desarrollo](https://img.shields.io/badge/Estado-En%20desarrollo-4338CA?style=flat-square)](#estado-del-proyecto)
[![Aplicación web progresiva](https://img.shields.io/badge/Aplicaci%C3%B3n-Web%20progresiva-0F766E?style=flat-square)](#tecnologías)

[Qué hace Edupe](#qué-hace-edupe) · [Cómo se usa](#cómo-se-usa) · [Tecnologías](#tecnologías) · [Hoja de ruta](#hoja-de-ruta)

</div>

---

## Qué hace Edupe

Edupe reúne el registro de asistencia del personal docente y administrativo, el seguimiento de la jornada laboral y los trámites de dirección en una aplicación web.

| Módulo | Alcance de la primera versión |
| :--- | :--- |
| 🔐 **Acceso y permisos** | Inicio de sesión con PIN de seis dígitos, cambio obligatorio de la clave temporal, recuperación por un responsable autorizado y permisos por operación. |
| 👥 **Institución y personal** | Alta, edición y desactivación de cuentas del personal, con conservación de su historial de asistencia. |
| 🗓️ **Horarios y calendario** | Configuración de jornadas, tolerancias y días no laborables. Los cambios tienen fecha de vigencia y se conservan las versiones anteriores. |
| 📱 **Punto QR** | Pantalla autorizada en el ingreso de la institución con un código que se renueva automáticamente y muestra el estado de conexión. |
| ✅ **Asistencia** | Marcación de entradas y salidas con hora del servidor, historial individual, detección de registros incompletos y correcciones con motivo obligatorio. |
| 📊 **Panel y reportes** | Seguimiento de la asistencia, filtros por periodo y estado, y exportación a Excel y PDF. |
| 🔔 **Agenda de dirección** | Recordatorios privados de trámites con vencimiento y repetición semanal o mensual. Las notificaciones Web Push forman parte del alcance pendiente. |
| 🧾 **Auditoría y operación** | Historial de cambios administrativos y de correcciones. El plan operativo incluye respaldos y verificación de su restauración. |

## Cómo se usa

1. **Dirección** registra al personal, configura el calendario y habilita el punto de marcación.
2. **El personal** inicia sesión, escanea el QR desde el celular y recibe una confirmación cuando se guarda la entrada o salida.
3. **Dirección** revisa registros incompletos, documenta las correcciones y descarga reportes del periodo.

Las correcciones conservan el valor original, el motivo, la fecha y la persona responsable. El servidor verifica los permisos y el alcance de la institución antes de ejecutar operaciones protegidas.

## Tecnologías

<div align="center">

![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-0E7490?style=flat-square&logo=tailwindcss&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-5A0FC8?style=flat-square&logo=pwa&logoColor=white)
![Java 21](https://img.shields.io/badge/Java%2021-E76F00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3D7A22?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

</div>

| Capa | Responsabilidad |
| :--- | :--- |
| **Aplicación web** | Angular, TypeScript y Tailwind CSS para el uso desde celulares y computadoras. La base PWA permite preparar la instalación desde el navegador. |
| **API** | Java 21 y Spring Boot para validar accesos, horarios, marcaciones y reportes. |
| **Datos** | PostgreSQL para almacenar personal, jornadas, asistencia y auditoría. |

## Estado del proyecto

**Implementado en la primera entrega:** acceso con PIN, gestión del personal, horarios con vigencia, punto QR, registros de asistencia, correcciones, exportaciones y agenda privada de dirección.

**En validación o pendiente:** escaneo QR e instalación y actualización de la PWA en dispositivos reales, mejoras en el panel de incidencias, Web Push y comprobaciones operativas de despliegue y respaldos.

## Hoja de ruta

- **Completar la V1** · Validar el flujo de asistencia con celulares, mejorar la revisión de incidencias y completar las notificaciones y la operación.
- **Incorporar más instituciones** · Evolucionar hacia una plataforma con acceso por subdominio, identidad propia por institución y datos aislados. La arquitectura SaaS está en planificación.
- **Ampliar la gestión institucional** · Evaluar para una segunda versión los permisos laborales, las justificaciones documentadas, las autorizaciones de salida anticipada, los comunicados y el chat.

---

<div align="center">

**Edupe** · Gestión institucional para la comunidad educativa

</div>

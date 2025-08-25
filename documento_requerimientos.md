# 📑 DOCUMENTO DE DEFINICIÓN DE REQUERIMIENTOS

---

## 🎯 Propósito

El objetivo de este documento es describir los **requerimientos funcionales** y **no funcionales** de un **sistema de gestión de reclamos y reparación de baches** 🕳️🚧.

Se busca **formalizar el proceso completo**, desde que un usuario reporta un reclamo hasta la intervención de una cuadrilla mediante una orden de trabajo y su respectiva reparación ✅.

---

## 🏙️ Fondo

Actualmente, cuando se reportan baches en la ciudad de **Bahía Blanca**, estos se registran en el **sistema de reparación** del **departamento de obras públicas**. A cada reclamo se le asigna un **número de identificación único**, y se almacena información como:

- 📍 **Calle**
- 📏 **Tamaño** (escala de 1 a 10)
- 📌 **Ubicación** (calzada, cuneta, etc.)
- 🗺️ **Distrito** (según dirección)
- ⏱️ **Prioridad de reparación** (determinada por el tamaño y riesgo)

👉 El proceso actual se realiza con **herramientas manuales** (planillas, hojas de cálculo, etc.), lo cual genera:

- ❌ **Pérdidas de información**
- 🔄 **Tareas duplicadas**
- 📉 **Falta de control y trazabilidad**
- ⚠️ **Datos incompletos o inconsistentes**
- 🔍 **Poca confiabilidad**

📲 Por lo tanto, **es necesario implementar un sistema digital** que centralice y organice estos registros, permitiendo el seguimiento completo de cada caso.

---

## 📌 Alcance

- 📝 **Recepción de reclamos:** Un ciudadano reporta un bache con descripción del problema.
- 🕳️ **Gestión del bache:** Se registran datos (ubicación, tamaño, observaciones) y se asocian reclamos.
- 🔍 **Asignación de inspecciones:** Un inspector evalúa el bache y agrega observaciones.
- 📑 **Generación de órdenes de trabajo:** Se genera una orden vinculada al bache inspeccionado.
- 👷 **Asignación de cuadrillas:** Una cuadrilla se asigna a la orden para ejecutar la reparación.
- 🛠️ **Registro de reparación:** Se documenta la intervención, fechas y observaciones.

---

## 📖 Definiciones

- 👤 **Usuario:** Persona que presenta un reclamo.
- 📢 **Reclamo:** Petición presentada respecto a un bache.
- 🕳️ **Bache:** Defecto en la vía pública que requiere reparación.
- 🕵️ **Inspector:** Empleado que analiza y documenta el estado del bache.
- 📑 **Orden de Trabajo:** Documento generado para coordinar la reparación.
- 👷 **Cuadrilla:** Grupo asignado a ejecutar la reparación.
- 🛠️ **Reparación:** Acción de arreglo físico del bache.
- 🆔 **ID:** Identificador único.
- 📲 **APP:** Aplicación digital del sistema.
- 🛰️ **GPS:** Sistema de posicionamiento global.

---

## ⚙️ Funcionalidades del Sistema

- 👤 **Módulo Usuario:** Registro básico de usuarios (actores del reclamo).
- 📢 **Módulo Reclamos:** Permite registrar reclamos y asociarlos a baches. ⚠️
- 🕳️ **Módulo Baches:** Registro de información detallada del bache (ubicación, tamaño, observaciones). Relación con reclamos e inspecciones. 🚧
- 🕵️ **Módulo Inspector:** Registro de observaciones y evaluación de baches. 🔍
- 📑 **Módulo Orden de Trabajo:** Generación de órdenes, asociación con cuadrillas y reparaciones. 📝
- 👷 **Módulo Cuadrilla:** Registro y asignación de cuadrillas a órdenes de trabajo. 👷‍♂️
- 🛠️ **Módulo Reparación:** Registro de reparaciones (fechas, estado, observaciones). 🔧

---

## ✅ Requerimientos Funcionales

- Registrar un **bache con ID único**, ubicación, tamaño (1-10), tipo y prioridad.
- Permitir que los usuarios **registren un reclamo** sobre un bache.
- Asignar **cuadrillas de reparación** con datos de su personal.
- Registrar **inspecciones** con observaciones.
- Asociar **reclamos múltiples** a un mismo bache.
- Registrar **horas trabajadas** y estado del bache.
- Generar **reportes por estado, barrio y fecha**.
- Asociar **daños reportados** con datos del ciudadano y monto económico 💰.
- Enviar **notificaciones/alertas** sobre reparaciones pendientes 🔔.
- Permitir la **consulta pública** del estado de reclamos 📊.
- Registrar **reparaciones asociadas** a una orden de trabajo, con fechas y observaciones.

---

## 🛡️ Requerimientos No Funcionales

- 🌐 **Accesibilidad:** Sistema accesible vía web (desktop y mobile).
- 🔎 **Trazabilidad:** Cada entidad (reclamo, bache, orden, reparación) debe ser rastreable.
- 🗄️ **Integridad de datos:** Toda reparación debe estar ligada a una orden de trabajo.
- 🖥️ **Simplicidad:** Interfaz amigable y clara para ciudadanos e inspectores.
- ⏱️ **Disponibilidad:** El sistema debe estar operativo al menos el **99,5% del tiempo**.
- 🔐 **Seguridad:** Acceso con credenciales seguras y cifrado de datos sensibles.

---

## 📌 Conclusión

Este documento establece de forma clara los requerimientos clave para un **sistema digital de seguimiento y reparación de baches**.

Se prioriza una visión centrada en el **ciudadano** 👥, garantizando **transparencia, eficiencia y confiabilidad** en el proceso de atención de reclamos.

> Como señalan Sommerville y Pressman, la correcta **definición de servicios y restricciones operativas** es esencial para el éxito de cualquier sistema de software 📚.


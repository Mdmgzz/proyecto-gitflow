# Proyecto GitFlow: Puesta en Producción Segura 🛡️

Este repositorio contiene la implementación práctica del modelo de trabajo **GitFlow**, diseñado para gestionar el ciclo de vida del software en entornos donde la estabilidad y la seguridad son críticas.

## 👥 Equipo de Trabajo - IES Martínez Montañés
* **Miguel Dominguez**: Arquitecto de Software y Gestión de Repositorio
* **[Nombre Integrante 2]**: Gestión de Releases y Estabilización
* **[Nombre Integrante 3]**: Especialista en Seguridad y Hotfixes

---

## 🏗️ Arquitectura de Ramas (Estrategia de PPS)
Siguiendo los principios de "Puesta en Producción Segura", el repositorio utiliza una estructura de aislamiento de código:

### Ramas de Larga Duración
* **`main`**: Representa el software en producción. Solo contiene código estable y etiquetado con versiones (tags).
* **`develop`**: Rama de integración donde se consolida el trabajo diario del equipo antes de ser considerado estable.

### Ramas de Soporte (Ciclo de Vida Temporal)
* **`feature/*`**: Desarrollo de nuevas funcionalidades de forma aislada para no bloquear el proyecto.
* **`release/*`**: Fase de "congelación de código" para ajustes finales y metadatos antes del despliegue.
* **`hotfix/*`**: Vía de emergencia para solucionar errores críticos detectados directamente en producción.

---

## 🛠️ Escenarios de Simulación para la Defensa
Durante la demostración práctica, el equipo ejecuta tres flujos críticos:

1.  **Escenario A (Feature)**: Creación e integración de una funcionalidad (ej: `autenticacion-login`).
2.  **Escenario B (Release)**: Preparación y cierre de la versión `v1.0.0`, sincronizando `main` y `develop`.
3.  **Escenario C (Hotfix)**: Resolución de un fallo de seguridad mediante un parche de emergencia aplicado a producción.

## 🔐 Valor Añadido en Seguridad
El uso de este modelo garantiza:
* **Trazabilidad**: Rastreo total desde la idea (feature) hasta el despliegue (tag).
* **Revisiones por Pares**: Control de calidad antes de integrar en ramas principales.
* **Recuperación (Rollback)**: Capacidad de revertir a una versión estable previa de forma inmediata gracias al etiquetado.

---
*Módulo: Puesta en Producción Segura (PPS) - Curso 25/26*
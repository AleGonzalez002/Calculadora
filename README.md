# Mini-Proyecto Ágil con Integración Continua

## 1. Prácticas de Calidad Aplicadas
* **Coding Standards (Linter):** Integración de `flake8` para auditar el código Python.
* **Flujo de trabajo con Pull Requests y Code Review:** Uso de ramas secundarias (`feature/multiplicacion`) y revisión explícita antes de la fusión.

## 2. Problemas que Evita
* **Errores de sintaxis y falta de estilo:** El linter detecta de forma inmediata problemas de formato (como la regla PEP 8 de dejar un salto de línea al final del archivo), impidiendo que lleguen a producción.
* **Integración tardía (Efecto "Big Bang"):** Subir cambios mediante Pull Requests asegura que el código se integre e inspeccione paso a paso.

## 3. Relación con los Conceptos de Clase
* **Evitar el "Big Bang":** En lugar de desarrollar toda la aplicación por separado y unirla el último día sufriendo incompatibilidades masivas, se realizan entregas pequeñas e integraciones continuas.
* **Reducción de retrabajo:** Al ejecutar validaciones automáticas mediante GitHub Actions en cada *push*, los fallos se identifican a los pocos segundos de ser creados, ahorrando tiempo de depuración posterior.
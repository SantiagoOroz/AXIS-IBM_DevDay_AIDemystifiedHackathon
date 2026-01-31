# AXIS - IBM Hackathon 2026

![IBM Watsonx](https://img.shields.io/badge/Powered%20by-IBM%20watsonx-blue)
![Status](https://img.shields.io/badge/Status-Hackathon%20MVP-orange)
![Agentic AI](https://img.shields.io/badge/Focus-Agentic%20AI-green)

> **El eje central entre el contrato pasivo y la gobernanza activa.**

## 📋 Resumen del Proyecto
**Axis** es un agente autónomo diseñado para eliminar la brecha entre los términos legales de una empresa y su operación diaria. Mientras que los contratos suelen quedar olvidados en archivos PDF, Axis actúa como un intermediario inteligente que "lee, razona y ejecuta". 

Utilizando modelos de lenguaje de última generación integrados en **watsonx.ai**, Axis no solo resume información, sino que toma decisiones proactivas: detecta incumplimientos, alerta sobre riesgos de renovación y automatiza tareas administrativas complejas.

---

## 🧠 Core Tecnológico (Stack IBM 2026)
Axis es una solución nativa de **Agentic AI** construida sobre la infraestructura de IBM:

* **Motor de Inteligencia (LLM):** `Llama-3.2-90b-vision-instruct` (vía **watsonx.ai**) - Responsable del razonamiento lógico, análisis de contexto y toma de decisiones.
* **Orquestador:** `watsonx Orchestrate` - El centro de mando que conecta a Axis con herramientas externas como Slack, Jira, Trello y Outlook.
* **Visión Artificial:** Utilizado para el procesamiento inteligente de facturas y contratos escaneados mediante las capacidades multimodales de Llama 3.2.

---

## ⚡ Capacidades Agénticas
A diferencia de un chatbot tradicional, Axis opera bajo una lógica de **autonomía configurada**:

1.  **Monitoreo Proactivo:** Analiza logs de uso y fechas de vencimiento para sugerir renegociaciones de contratos antes de que ocurran aumentos automáticos.
2.  **Validación de Facturas (Bridge):** Detecta discrepancias de precios en facturas mediante visión artificial y abre disputas en Jira de forma autónoma.
3.  **Governance Guardian:** Intervención en tiempo real en canales de comunicación si un empleado promete condiciones que violan los T&C estándar.
4.  **Onboarding de Contexto:** Al detectar la integración de nuevos miembros al equipo, Axis gestiona permisos en Drive y crea tareas de inducción en Trello automáticamente.

---

## 🛠️ Contenido del Repositorio
Este repositorio funciona como el centro de documentación y arquitectura de la solución:
* `/workflows`: Diagramas de flujo de la lógica agéntica y orquestación de skills en Orchestrate.
* `/prompts`: Configuración de los prompts de sistema para el modelo Llama-3.2.
* `/docs`: Guías de implementación y casos de uso de negocio para la demo.

---

## 👥 Equipo
Proyecto desarrollado para la **IBM Hackathon 2026** por:

* **Santiago Oroz** - [santiago.oroz1510@gmail.com](mailto:santiago.oroz1510@gmail.com)
* **Renata Berho** - [renaberho2@gmail.com](mailto:renaberho2@gmail.com)
* **Milagros Argañin** - [miliarganin3@gmail.com](mailto:miliarganin3@gmail.com)

---
*Axis demuestra cómo la potencia de los modelos abiertos en watsonx.ai permite transformar el cumplimiento legal en una ventaja operativa.*

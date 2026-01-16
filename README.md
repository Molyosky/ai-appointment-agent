
# 🤖 AI Appointment Booking Agent

Un agente de Inteligencia Artificial autónomo capaz de gestionar agendas médicas, verificar disponibilidad en tiempo real y confirmar citas a través de WhatsApp.

## 🚀 Tecnologías Usadas
* **Core:** n8n (Workflow Automation)
* **Infraestructura:** Docker & Docker Compose
* **Inteligencia Artificial:** Google Gemini 2.5 Flash (Function Calling)
* **Integraciones:** Google Calendar API (OAuth2) & WhatsApp (via WAHA)

## ⚙️ Arquitectura
El sistema opera mediante contenedores Docker interconectados:
1.  **n8n:** Orquesta la lógica, gestiona la memoria de la conversación y conecta las APIs.
2.  **WAHA:** Provee la interfaz HTTP para enviar/recibir mensajes de WhatsApp.

## 🛠️ Instalación (Local)
1.  Clonar el repositorio.
2.  Configurar credenciales en n8n (Google Cloud & Gemini).
3.  Ejecutar el entorno:
    ```bash
    docker compose up -d
    ```

## 📋 Funcionalidades
* Lectura de disponibilidad en tiempo real (evita conflictos de horario).
* Manejo de memoria conversacional (recuerda el contexto del paciente).
* Agendamiento automático en Google Calendar.
* Respuestas en lenguaje natural.

---
*Desarrollado por Dereck Galán - Ingeniería en Sistemas PUCE*

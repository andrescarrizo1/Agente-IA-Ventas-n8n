# 🤖 Agente IA de Ventas Grau.AD (Workflow n8n)

Este repositorio contiene un flujo de trabajo (workflow) de n8n diseñado para funcionar como un **Agente de Inteligencia Artificial de Ventas** para la cualificación automática de leads y la gestión de procesos.

## 💡 Descripción del Workflow

El agente, llamado "Agente Grau.AD 🏔️", opera como un chatbot de ventas guiado, con el objetivo principal de conseguir que los usuarios reserven una auditoría gratuita de IA.

### ⚙️ Componentes Clave (Nodos)

| Nombre del Nodo (JSON) | Función Principal |
|---|---|
| `chatTrigger` | Inicia la conversación cuando un usuario envía un mensaje. |
| `Agente Grau.AD (WEB)` | Agente IA Principal (usa Gemini 1.5 Pro). Contiene la lógica central y la Guía de Ventas. |
| `Google Vertex Chat Model` | El cerebro del Agente, usa **Gemini 1.5 Pro** para la conversación y las respuestas. |
| `Postgres Chat Memory` | Almacena la conversación, permitiendo al Agente recordar el contexto. |
| `Google Sheets` | Se usa para **registrar y cualificar leads** (Nombre, Correo, Empresa) automáticamente. |
| `Gmail` | Utilizado para **notificar al consultor** y enviar un **resumen personalizado** al usuario. |

### 🎯 Valor de la Solución

1.  **Captura de Leads:** El Agente cualifica a los prospectos según su modelo de negocio.
2.  **Venta Guiada:** Resuelve objeciones sobre el coste y seguridad de la IA de forma estructurada.
3.  **Automatización:** El flujo automatiza tres acciones críticas (guardar lead, notificar a ventas y enviar resumen) simultáneamente, ahorrando tiempo y aumentando la eficiencia comercial.

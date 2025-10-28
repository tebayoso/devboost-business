# Ejercicio: Diseño de Chatbot

## Información del Proyecto
- **Nombre del bot:** _______________
- **Área de aplicación:**
  - [ ] Soporte al cliente
  - [ ] Ventas
  - [ ] Recursos Humanos
  - [ ] Otro: _______________
- **Diseñador:** _______________
- **Fecha:** _______________

---

## 1. Definición del Caso de Uso

### Objetivo del Chatbot


### Usuarios objetivo
- Perfil demográfico:
- Nivel técnico:
- Expectativas:

### Problemas que resuelve
1.
2.
3.

---

## 2. Top 5 Preguntas Frecuentes

### FAQ 1
**Pregunta:**

**Respuesta del bot:**


**Variaciones de la pregunta:**
-
-

---

### FAQ 2
**Pregunta:**

**Respuesta del bot:**


**Variaciones de la pregunta:**
-
-

---

### FAQ 3
**Pregunta:**

**Respuesta del bot:**


**Variaciones de la pregunta:**
-
-

---

### FAQ 4
**Pregunta:**

**Respuesta del bot:**


**Variaciones de la pregunta:**
-
-

---

### FAQ 5
**Pregunta:**

**Respuesta del bot:**


**Variaciones de la pregunta:**
-
-

---

## 3. Flujo de Conversación

### Saludo Inicial
```
Bot: ¡Hola! 👋 Soy [NOMBRE], tu asistente virtual.
¿En qué puedo ayudarte hoy?

Opciones:
1. [Opción 1]
2. [Opción 2]
3. [Opción 3]
4. Hablar con un humano
```

### Flujo Principal
```
Usuario: [Pregunta]
    ↓
Bot analiza intención
    ↓
¿Confianza > 80%?
    ├─ SÍ → Responde directamente
    └─ NO → Pide aclaración
         ↓
    Usuario aclara
         ↓
    Bot responde o escala
```

### Manejo de Casos Difíciles
```
Si el bot no entiende:
1. Pedir reformular (máx 2 veces)
2. Ofrecer opciones relacionadas
3. Opción de contacto humano
```

---

## 4. Criterios de Escalamiento a Humano

### Escalamiento Automático
- [ ] Pregunta compleja detectada
- [ ] Usuario frustrado (palabras clave: "no sirve", "terrible")
- [ ] 3+ intentos fallidos de comprensión
- [ ] Solicitud explícita del usuario
- [ ] Tema fuera de scope

### Proceso de Escalamiento
1. Bot: "Veo que necesitas ayuda especializada. Te voy a conectar con un agente humano."
2. Recolectar información:
   - Nombre
   - Email/Teléfono
   - Resumen del problema
3. Crear ticket y notificar agente
4. Estimado de espera

---

## 5. Personalidad del Bot

### Tono de voz
- [ ] Profesional
- [ ] Amigable
- [ ] Casual
- [ ] Técnico
- [ ] Empático

### Características
- Usa emojis: [ ] Sí [ ] No
- Tutea o trata de usted: _______
- Respuestas: [ ] Concisas [ ] Detalladas
- Humor: [ ] Sí [ ] No

### Ejemplo de respuesta con personalidad


---

## 6. Integgraciones Necesarias

### Sistemas
- [ ] CRM (ej: Salesforce)
- [ ] Base de conocimientos
- [ ] Sistema de tickets
- [ ] Base de datos de productos
- [ ] Otro: _______________

### APIs requeridas
1.
2.
3.

---

## 7. Métricas de Éxito

### KPIs Cuantitativos
- **Tasa de resolución:** _____%
- **Tiempo promedio de respuesta:** ____ segundos
- **Satisfacción del usuario (CSAT):** ____/5
- **Conversaciones completadas sin escalamiento:** _____%
- **Volumen de conversaciones atendidas:** ____ /día

### KPIs Cualitativos
- Feedback de usuarios
- Tipos de problemas resueltos
- Áreas de mejora identificadas

---

## 8. Diagrama de Flujo

```
[Inicio]
   ↓
[Saludo]
   ↓
[Usuario pregunta]
   ↓
[¿Entendió?] ─ NO ─→ [Pedir aclaración] ─→ [¿Entendió?]
   │                                            │
   SÍ                                          NO (3x)
   ↓                                            ↓
[Buscar respuesta]                        [Escalar a humano]
   ↓
[¿Tiene respuesta?]
   │
   ├─ SÍ ─→ [Mostrar respuesta] ─→ [¿Resolvió?]
   │                                    │
   │                              SÍ ──┴── NO
   │                               ↓        ↓
   └─ NO ──────────────────→ [Escalar] [Más ayuda]
                                          ↓
                                    [Reiniciar]
```

---

## 9. Implementación Técnica

### Stack Propuesto
- **Plataforma de IA:** _______________
- **Frontend:** _______________
- **Backend:** _______________
- **Base de datos:** _______________

### Presupuesto Estimado
- Desarrollo: $_______
- APIs/Servicios mensuales: $_______
- Mantenimiento mensual: $_______

### Timeline
- Diseño: _____ semanas
- Desarrollo: _____ semanas
- Testing: _____ semanas
- Lanzamiento: _____

---

## 10. Plan de Mejora Continua

### Fase 1 (MVP)
- Responder FAQs básicas
- Escalamiento a humanos
- Métricas básicas

### Fase 2 (Optimización)
- Análisis de conversaciones
- Refinar respuestas
- Agregar más intenciones

### Fase 3 (Avanzado)
- Personalización por usuario
- Proactividad
- Integración completa

---

## Notas Adicionales


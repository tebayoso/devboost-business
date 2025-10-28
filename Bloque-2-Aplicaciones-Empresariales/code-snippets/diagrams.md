# Diagramas Visuales - Bloque 2: Aplicaciones Empresariales

## 1. Automatización Inteligente - Flujo de Procesos

```mermaid
flowchart TD
    Start[Entrada de Tarea] --> Classify{IA Clasifica<br/>Tipo de Tarea}
    Classify -->|Repetitiva| Auto1[Automatización<br/>Total]
    Classify -->|Semi-compleja| Auto2[Asistencia IA<br/>+ Humano]
    Classify -->|Compleja| Human[Escalamiento<br/>a Experto]

    Auto1 --> Execute[IA Ejecuta]
    Execute --> Validate{Validación<br/>Automática}
    Validate -->|OK| Complete[✓ Completado]
    Validate -->|Error| Auto2

    Auto2 --> Assist[IA Sugiere]
    Assist --> HumanDecision[Humano Decide]
    HumanDecision --> Execute2[Ejecutar Acción]
    Execute2 --> Complete

    Human --> Expert[Experto Maneja]
    Expert --> Learn[IA Aprende<br/>del Proceso]
    Learn --> Complete

    style Complete fill:#4CAF50,stroke:#2E7D32,color:#fff
    style Execute fill:#2196F3,stroke:#1976D2,color:#fff
```

## 2. Arquitectura de Chatbot Empresarial

```mermaid
graph TB
    subgraph "Frontend"
        Widget[Widget de Chat]
        Mobile[App Móvil]
        Web[Dashboard Web]
    end

    subgraph "Capa de Orquestación"
        Router[Router de Intenciones]
        Context[Gestor de Contexto]
        Analytics[Analytics en Tiempo Real]
    end

    subgraph "Capa de IA"
        NLP[NLP Engine]
        LLM[LLM<br/>GPT-4/Claude]
        KB[Base de<br/>Conocimientos]
        Vector[(Vector DB)]
    end

    subgraph "Integraciones"
        CRM[(CRM)]
        Tickets[(Sistema<br/>Tickets)]
        Docs[(Documentación)]
    end

    Widget --> Router
    Mobile --> Router
    Web --> Router

    Router --> NLP
    Router --> Context
    NLP --> LLM
    LLM --> KB
    KB --> Vector

    Router --> Analytics
    Context --> CRM
    Context --> Tickets
    KB --> Docs

    style LLM fill:#4CAF50,stroke:#2E7D32,color:#fff
```

## 3. Embudo de Ventas con IA

```mermaid
%%{init: {'theme':'base', 'flowchart': {'curve': 'basis'}}}%%
graph TD
    A[1000 Leads] -->|IA Score| B{Calificación}
    B -->|Alta: 300| C[Leads Calientes]
    B -->|Media: 400| D[Leads Tibios]
    B -->|Baja: 300| E[Leads Fríos]

    C -->|IA Personaliza| F[Email Automático<br/>Personalizado]
    F --> G[150 Responden]
    G -->|IA Analiza| H[Detección de<br/>Oportunidad]
    H --> I[75 Reuniones]
    I --> J[45 Propuestas]
    J --> K[25 Cierres]

    D -->|Nurturing IA| L[Contenido<br/>Automático]
    L --> M[+100 Calientes]
    M --> C

    E -->|IA Monitorea| N[Señales de<br/>Intención]
    N --> O[+50 Tibios]
    O --> D

    style K fill:#4CAF50,stroke:#2E7D32,color:#fff,stroke-width:3px
    style C fill:#FF9800,stroke:#F57C00,color:#fff
```

## 4. Impacto de IA en Productividad por Rol

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor':'#2196F3'}}}%%
graph LR
    subgraph "Sin IA"
        D1[Desarrollador<br/>5 proyectos/mes]
        V1[Vendedor<br/>20 leads/semana]
        S1[Soporte<br/>50 tickets/día]
        M1[Marketer<br/>10 campañas/mes]
    end

    subgraph "Con IA"
        D2[Desarrollador<br/>11 proyectos/mes<br/>+120%]
        V2[Vendedor<br/>35 leads/semana<br/>+75%]
        S2[Soporte<br/>300 tickets/día<br/>+500%]
        M2[Marketer<br/>25 campañas/mes<br/>+150%]
    end

    D1 -.IA.-> D2
    V1 -.IA.-> V2
    S1 -.IA.-> S2
    M1 -.IA.-> M2

    style D2 fill:#4CAF50,stroke:#2E7D32,color:#fff
    style V2 fill:#4CAF50,stroke:#2E7D32,color:#fff
    style S2 fill:#4CAF50,stroke:#2E7D32,color:#fff
    style M2 fill:#4CAF50,stroke:#2E7D32,color:#fff
```

## 5. Modelo Híbrido de Soporte (IA + Humano)

```mermaid
stateDiagram-v2
    [*] --> Recepción: Cliente contacta
    Recepción --> Nivel1: Triage automático

    Nivel1: Bot IA (60-70%)
    Nivel1 --> Resuelto: Pregunta simple
    Nivel1 --> Nivel2: Necesita humano

    Nivel2: Agente + IA (25-30%)
    Nivel2 --> Resuelto: Caso estándar
    Nivel2 --> Nivel3: Caso complejo

    Nivel3: Especialista (5-10%)
    Nivel3 --> Resuelto: Solución experta

    Resuelto --> Feedback: CSAT Survey
    Feedback --> [*]: Aprende y mejora

    note right of Nivel1
        IA maneja:
        - FAQs
        - Estado de pedidos
        - Info productos
        - Reseteos simples
    end note

    note right of Nivel2
        Agente con IA:
        - Historial automático
        - Sugerencias IA
        - Respuestas rápidas
    end note
```

## 6. Pipeline de Desarrollo con IA

```mermaid
timeline
    title Ciclo de Desarrollo con IA
    section Planificación
        Historias de usuario : IA genera casos de uso
        Estimaciones : IA predice tiempos
    section Desarrollo
        Código : GitHub Copilot asiste
        Revisión : IA detecta code smells
        Documentación : Auto-generada
    section Testing
        Tests unitarios : IA genera tests
        Tests integración : Cobertura automática
        QA : IA identifica bugs
    section Deployment
        CI/CD : Pipeline optimizado con IA
        Monitoreo : Detección proactiva de issues
        Hotfixes : IA prioriza y sugiere fixes
```

## 7. Lead Scoring con Machine Learning

```mermaid
graph TD
    subgraph "Datos de Entrada"
        A1[Datos Demográficos]
        A2[Comportamiento Web]
        A3[Email Engagement]
        A4[Social Media]
        A5[Firmográficos]
    end

    subgraph "Modelo ML"
        B[Feature Engineering]
        C[Modelo Predictivo]
        D[Score 0-100]
    end

    subgraph "Acción"
        E1[Alta: 80-100<br/>Contactar Ya]
        E2[Media: 50-79<br/>Nurturing]
        E3[Baja: 0-49<br/>Monitorear]
    end

    A1 --> B
    A2 --> B
    A3 --> B
    A4 --> B
    A5 --> B
    B --> C
    C --> D
    D --> E1
    D --> E2
    D --> E3

    E1 --> F[Vendedor<br/>+ Script IA]
    E2 --> G[Campaña<br/>Automatizada]
    E3 --> H[Retargeting<br/>Ads]

    style E1 fill:#4CAF50,stroke:#2E7D32,color:#fff
    style E2 fill:#FF9800,stroke:#F57C00,color:#fff
    style E3 fill:#2196F3,stroke:#1976D2,color:#fff
```

## 8. Automatización de Marketing de Contenidos

```mermaid
flowchart LR
    A[Estrategia de Contenido] --> B[IA Genera<br/>Ideas]
    B --> C{Tipo de<br/>Contenido}

    C -->|Blog| D1[IA Escribe<br/>Draft]
    C -->|Social| D2[IA Crea<br/>Posts]
    C -->|Email| D3[IA Personaliza<br/>Campañas]
    C -->|Video| D4[IA Genera<br/>Scripts]

    D1 --> E1[Humano Edita<br/>y Aprueba]
    D2 --> E1
    D3 --> E1
    D4 --> E1

    E1 --> F[Publicación<br/>Automática]
    F --> G[IA Analiza<br/>Performance]
    G --> H{¿Funciona?}

    H -->|Sí| I[Escalar<br/>Estrategia]
    H -->|No| J[Ajustar<br/>Approach]

    I --> A
    J --> A

    style E1 fill:#FF9800,stroke:#F57C00,color:#fff
    style I fill:#4CAF50,stroke:#2E7D32,color:#fff
```

## 9. Análisis de Sentimiento en Tiempo Real

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor':'#2196F3'}}}%%
pie title Distribución de Sentimiento - Análisis de 10,000 Comentarios
    "😊 Positivo (65%)" : 6500
    "😐 Neutral (25%)" : 2500
    "😠 Negativo (10%)" : 1000
```

## 10. ROI de Implementaciones de IA por Área

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor':'#4CAF50'}}}%%
graph TB
    subgraph "ROI a 6 Meses"
        A[Chatbot<br/>Soporte<br/>245%]
        B[Lead Scoring<br/>Ventas<br/>380%]
        C[Code Assistant<br/>Desarrollo<br/>290%]
        D[Content Gen<br/>Marketing<br/>320%]
    end

    subgraph "ROI a 12 Meses"
        E[Detección Fraude<br/>Fintech<br/>560%]
        F[Mantenimiento<br/>Manufactura<br/>850%]
        G[BI Analytics<br/>Datos<br/>410%]
    end

    style A fill:#4CAF50,stroke:#2E7D32,color:#fff
    style B fill:#4CAF50,stroke:#2E7D32,color:#fff
    style C fill:#4CAF50,stroke:#2E7D32,color:#fff
    style D fill:#4CAF50,stroke:#2E7D32,color:#fff
    style E fill:#2196F3,stroke:#1976D2,color:#fff
    style F fill:#2196F3,stroke:#1976D2,color:#fff
    style G fill:#2196F3,stroke:#1976D2,color:#fff
```

## 11. Customer Journey con IA

```mermaid
journey
    title Experiencia del Cliente Potenciada con IA
    section Descubrimiento
      Visita web: 5: Cliente
      Chatbot saluda: 5: IA
      Recomendaciones personalizadas: 5: IA
    section Consideración
      Descarga contenido: 4: Cliente
      Lead scoring automático: 5: IA
      Email personalizado: 5: IA, Ventas
    section Decisión
      Demo interactiva: 5: Cliente, IA
      Propuesta generada por IA: 4: Ventas, IA
      Negociación: 5: Ventas, Cliente
    section Compra
      Proceso automático: 5: IA
      Onboarding personalizado: 5: IA, Cliente
    section Post-venta
      Soporte 24/7: 5: IA, Cliente
      Upsell inteligente: 4: IA, Cliente
      Feedback y mejora: 5: IA, Todos
```

## 12. Comparativa: Con y Sin IA en Soporte

```mermaid
gantt
    title Resolución de Ticket: Tradicional vs IA
    dateFormat X
    axisFormat %H:%M

    section Sin IA
    Cliente espera        :0, 24h
    Asignación manual     :24h, 2h
    Agente investiga      :26h, 4h
    Respuesta enviada     :30h, 1h
    Follow-up             :31h, 2h
    Total: 33 horas       :milestone, 33h

    section Con IA
    Bot responde          :0, 30s
    Solución automática   :30s, 30s
    CSAT                  :1min, 1min
    Total: 2 minutos      :milestone, 2min
```

## 13. Arquitectura de Sistema de IA Generativa para Empresas

```mermaid
C4Context
    title Arquitectura de IA Generativa Empresarial

    Person(user, "Usuario", "Empleado o Cliente")

    System_Boundary(app, "Aplicación Empresarial") {
        Container(webapp, "Web App", "React", "Frontend")
        Container(api, "API Gateway", "Node.js", "Orquestación")
        Container(ai, "IA Engine", "LangChain", "Procesamiento IA")
    }

    System_Ext(llm, "LLM Provider", "OpenAI/Anthropic")
    System_Ext(vector, "Vector DB", "Pinecone")
    SystemDb(db, "Base de Datos", "PostgreSQL")
    System_Ext(crm, "CRM", "Salesforce")

    Rel(user, webapp, "Usa")
    Rel(webapp, api, "Llama API")
    Rel(api, ai, "Procesa")
    Rel(ai, llm, "Consulta")
    Rel(ai, vector, "Busca contexto")
    Rel(api, db, "Lee/Escribe")
    Rel(api, crm, "Integra")
```

## Cómo Usar Estos Diagramas

### Renderizar en Markdown
GitHub, GitLab, y muchas herramientas soportan Mermaid nativamente:
````markdown
```mermaid
graph TD
    A --> B
```
````

### Herramientas Online
- [Mermaid Live Editor](https://mermaid.live)
- [Mermaid Chart](https://www.mermaidchart.com)

### Exportar
- PNG/SVG para presentaciones
- PDF para documentos
- Código embebido en HTML

### Personalizar
Todos los diagramas pueden modificarse cambiando:
- Colores: `style NodeID fill:#COLOR`
- Textos: Edita directamente
- Estructura: Agrega o quita nodos

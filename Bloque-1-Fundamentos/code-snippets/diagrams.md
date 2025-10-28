# Diagramas Visuales - Bloque 1: Fundamentos

## 1. Evolución del Mercado de IA (2020-2025)

```mermaid
graph LR
    A[2020<br/>$30B] -->|+40%| B[2021<br/>$42B]
    B -->|+45%| C[2022<br/>$61B]
    C -->|+50%| D[2023<br/>$91B]
    D -->|+38%| E[2025<br/>$126B]

    style E fill:#4CAF50,stroke:#2E7D32,color:#fff
```

## 2. Comparativa de Modelos LLM (2025)

```mermaid
mindmap
  root((Modelos LLM<br/>2025))
    GPT-4
      Versatilidad
      Razonamiento
      Ecosistema
    Claude 3
      Contexto largo
      Precisión
      Análisis profundo
    Grok
      Tiempo real
      Twitter/X
      Actualidad
    Gemini
      Multimodal
      Google Suite
      Búsqueda
    LLaMA
      Open Source
      Personalizable
      On-premise
```

## 3. Framework de Evaluación de ROI

```mermaid
flowchart TD
    Start[Inicio] --> Identify[Identificar Problema]
    Identify --> Data{¿Hay datos<br/>suficientes?}
    Data -->|No| DataCollect[Recolectar Datos]
    DataCollect --> Data
    Data -->|Sí| Viable{¿Viabilidad<br/>técnica?}
    Viable -->|No| Alternative[Buscar alternativas]
    Viable -->|Sí| ROI[Calcular ROI]
    ROI --> Cost[Estimar Costos]
    ROI --> Benefits[Estimar Beneficios]
    Cost --> Compare{ROI > 100%<br/>a 12 meses?}
    Benefits --> Compare
    Compare -->|No| Reevaluate[Re-evaluar o descartar]
    Compare -->|Sí| Pilot[Implementar MVP]
    Pilot --> Measure[Medir Resultados]
    Measure --> Success{¿Exitoso?}
    Success -->|Sí| Scale[Escalar]
    Success -->|No| Iterate[Iterar o Pivotar]
    Iterate --> Pilot

    style Start fill:#2196F3,stroke:#1976D2,color:#fff
    style Scale fill:#4CAF50,stroke:#2E7D32,color:#fff
    style Reevaluate fill:#F44336,stroke:#C62828,color:#fff
```

## 4. IA Tradicional vs IA Generativa

```mermaid
graph TD
    subgraph "IA Tradicional"
        A1[Entrada de Datos] --> B1[Modelo Entrenado]
        B1 --> C1{Tipo de Tarea}
        C1 -->|Clasificar| D1[Categoría A o B]
        C1 -->|Predecir| D2[Valor Numérico]
        C1 -->|Reconocer| D3[Patrón Identificado]
    end

    subgraph "IA Generativa"
        A2[Prompt/Instrucción] --> B2[LLM]
        B2 --> C2{Genera}
        C2 --> D4[Texto Nuevo]
        C2 --> D5[Código]
        C2 --> D6[Imágenes]
        C2 --> D7[Razonamiento]
    end

    style A1 fill:#FFC107,stroke:#F57C00
    style A2 fill:#4CAF50,stroke:#2E7D32
```

## 5. Aplicaciones de IA por Industria

```mermaid
%%{init: {'theme':'base', 'themeVariables': { 'primaryColor':'#2196F3'}}}%%
pie title Adopción de IA por Sector (2025)
    "Tecnología" : 25
    "Finanzas" : 20
    "Salud" : 15
    "Retail" : 12
    "Manufactura" : 10
    "Marketing" : 8
    "Educación" : 5
    "Otros" : 5
```

## 6. Ciclo de Adopción de IA en Empresa

```mermaid
journey
    title Viaje de Adopción de IA en la Empresa
    section Descubrimiento
      Awareness: 3: Equipo
      Investigación inicial: 4: Equipo
      Identificar casos de uso: 5: Equipo, Líderes
    section Evaluación
      Análisis de viabilidad: 4: Líderes, IT
      Cálculo de ROI: 5: Finanzas, Líderes
      Aprobación presupuesto: 3: Ejecutivos
    section Implementación
      MVP/Piloto: 5: IT, Equipo
      Testing: 4: IT, Usuarios
      Iteración: 5: IT, Equipo
    section Escalamiento
      Rollout gradual: 4: IT, Todos
      Capacitación: 5: Todos
      Optimización continua: 5: IT, Equipo
    section Madurez
      Expansión a más casos: 5: Todos
      Cultura de IA: 5: Todos
```

## 7. Stack Tecnológico de IA

```mermaid
graph TB
    subgraph "Capa de Presentación"
        UI[Aplicaciones Web/Móvil]
        Dash[Dashboards]
        Chat[Interfaces de Chat]
    end

    subgraph "Capa de Aplicación"
        API[APIs REST]
        Logic[Lógica de Negocio]
        Auth[Autenticación]
    end

    subgraph "Capa de IA/ML"
        LLM[LLMs<br/>GPT-4, Claude]
        ML[Modelos ML Custom]
        Vector[Vector Databases]
    end

    subgraph "Capa de Datos"
        DB[(Base de Datos)]
        DL[(Data Lake)]
        Cache[(Cache)]
    end

    UI --> API
    Dash --> API
    Chat --> API
    API --> Logic
    Logic --> LLM
    Logic --> ML
    LLM --> Vector
    Logic --> DB
    ML --> DL
    API --> Cache

    style LLM fill:#4CAF50,stroke:#2E7D32,color:#fff
    style ML fill:#2196F3,stroke:#1976D2,color:#fff
```

## 8. Consideraciones Éticas y Riesgos

```mermaid
mindmap
  root((Consideraciones<br/>IA))
    Privacidad
      GDPR
      CCPA
      Datos sensibles
      Consentimiento
    Sesgos
      Datos de entrenamiento
      Decisiones justas
      Auditorías
      Diversidad
    Transparencia
      Explicabilidad
      Trazabilidad
      Documentación
      Accountability
    Seguridad
      Adversarial attacks
      Data poisoning
      Model stealing
      Access control
    Impacto Social
      Desplazamiento laboral
      Reentrenamiento
      Transición justa
      Nuevos roles
```

## 9. Cálculo de ROI - Ejemplo Visual

```mermaid
graph LR
    A[Situación Actual] -->|Costos| B[Análisis]
    A -->|Tiempo| B
    B --> C{Implementar IA}
    C -->|Inversión Inicial| D[Costos IA]
    C -->|Ahorro Tiempo| E[Beneficios]
    C -->|Reducción Errores| E
    C -->|Aumento Productividad| E
    D --> F[ROI = <br/>Beneficios - Costos<br/> / Costos × 100]
    E --> F
    F --> G{¿ROI > 100%?}
    G -->|Sí| H[✓ Implementar]
    G -->|No| I[✗ Reevaluar]

    style H fill:#4CAF50,stroke:#2E7D32,color:#fff
    style I fill:#F44336,stroke:#C62828,color:#fff
```

## 10. Matriz de Priorización de Casos de Uso

```mermaid
quadrantChart
    title Priorización de Casos de Uso de IA
    x-axis Baja Viabilidad --> Alta Viabilidad
    y-axis Bajo Impacto --> Alto Impacto
    quadrant-1 Implementar Ya
    quadrant-2 Planificar
    quadrant-3 Postergar
    quadrant-4 Quick Wins
    Chatbot Soporte: [0.8, 0.9]
    Lead Scoring: [0.7, 0.8]
    Análisis Datos: [0.6, 0.7]
    Detección Fraude: [0.5, 0.9]
    Generación Código: [0.9, 0.6]
    Mantenimiento Predictivo: [0.4, 0.8]
```

## Cómo Usar Estos Diagramas

### En Presentaciones
1. Copia el código Mermaid
2. Usa herramientas como:
   - [Mermaid Live Editor](https://mermaid.live)
   - [GitHub](https://github.com) (soporte nativo)
   - [Notion](https://notion.so)
   - [Obsidian](https://obsidian.md)

### Exportar como Imagen
- Mermaid Live: Exporta a PNG, SVG, PDF
- GitHub: Screenshots
- Herramientas CLI: `mmdc` (mermaid-cli)

### Personalizar
Modifica los colores, textos y estructura según tu necesidad en el código Mermaid.

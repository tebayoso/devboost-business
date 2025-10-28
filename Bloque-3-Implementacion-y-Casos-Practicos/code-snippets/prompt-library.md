# Biblioteca de Prompts Reutilizables

Esta biblioteca contiene prompts probados y optimizados para casos de uso comunes en negocios.

---

## Categoría: Análisis de Datos

### Prompt: Análisis FODA (SWOT)
```
Actúa como un consultor estratégico con 15 años de experiencia.

Analiza la siguiente información y genera un análisis FODA completo:

[CONTEXTO/DATOS]

Estructura tu análisis así:

1. **Fortalezas** (Factores internos positivos)
   - Lista mínimo 4 fortalezas
   - Prioriza por impacto

2. **Oportunidades** (Factores externos positivos)
   - Lista mínimo 4 oportunidades
   - Incluye tendencias de mercado

3. **Debilidades** (Factores internos negativos)
   - Lista mínimo 4 debilidades
   - Sé objetivo y específico

4. **Amenazas** (Factores externos negativos)
   - Lista mínimo 4 amenazas
   - Considera competencia y regulación

5. **Recomendaciones Estratégicas**
   - 3 acciones prioritarias
   - Timeline sugerido
   - Recursos necesarios

Usa formato markdown con bullets y negritas para destacar puntos clave.
```

### Prompt: Análisis de Sentimiento de Feedback
```
Eres un analista de experiencia del cliente.

Analiza los siguientes comentarios de clientes y genera un reporte que incluya:

Comentarios:
[LISTA DE COMENTARIOS]

Reporte:
1. **Distribución de Sentimiento**
   - Positivo: X%
   - Neutral: X%
   - Negativo: X%

2. **Temas Principales**
   - Lista los 5 temas más mencionados
   - Incluye frecuencia

3. **Insights Clave**
   - 3 hallazgos principales
   - Patrones identificados

4. **Acciones Recomendadas**
   - Prioridad alta (urgente)
   - Prioridad media
   - Prioridad baja

Formato: Profesional, conciso, orientado a acción.
```

---

## Categoría: Generación de Contenido

### Prompt: Email de Ventas Personalizado
```
Eres un experto en ventas B2B con historial de 40% de conversión.

Escribe un email de seguimiento para:

**Contexto:**
- Prospecto: [NOMBRE/EMPRESA]
- Industria: [INDUSTRIA]
- Acción previa: [Descargó whitepaper / Visitó demo / etc.]
- Producto: [TU PRODUCTO]
- Valor principal: [BENEFICIO CLAVE]

**Requisitos del email:**
- Máximo 150 palabras
- Subject line llamativo
- Personalizado (menciona su industria/dolor)
- Un solo CTA claro
- Tono consultivo, no vendedor
- No mencionar precio

**Formato:**
Subject: [...]

Hola [NOMBRE],

[Cuerpo del email]

[Firma]
```

### Prompt: Post para LinkedIn
```
Crea un post para LinkedIn sobre [TEMA] que:

**Objetivo:** [Educar / Generar engagement / Thought leadership]

**Requisitos:**
- Longitud: 150-200 palabras
- Comienza con un hook que detenga el scroll
- Incluye 1-2 estadísticas impactantes
- Usa formato de lista o párrafos cortos
- Termina con pregunta para engagement
- 3-5 hashtags relevantes
- Tono: Profesional pero accesible

**Contexto:**
- Audiencia: [PERFIL]
- Mensaje clave: [INSIGHT PRINCIPAL]
- CTA (si aplica): [ACCIÓN DESEADA]

Evita:
- Lenguaje de ventas
- Clichés corporativos
- Más de 3 emojis
```

---

## Categoría: Programación

### Prompt: Generación de Código con Explicación
```
Eres un ingeniero de software senior especializado en [LENGUAJE].

Tarea: [DESCRIPCIÓN DE LA FUNCIÓN/FEATURE]

Requisitos:
- Lenguaje: [LENGUAJE]
- Framework (si aplica): [FRAMEWORK]
- Input: [TIPO Y DESCRIPCIÓN]
- Output: [TIPO Y DESCRIPCIÓN]
- Restricciones: [CUALQUIER LIMITACIÓN]

Por favor genera:

1. **Código completo y funcional**
   - Incluye imports necesarios
   - Manejo de errores
   - Validación de inputs
   - Comentarios en código

2. **Explicación línea por línea**
   - Qué hace cada sección
   - Por qué se eligió ese approach

3. **Casos de uso**
   - 3 ejemplos de uso
   - Incluyendo edge cases

4. **Testing**
   - Casos de prueba sugeridos
   - Código de tests unitarios

Formato: Código en bloques markdown con sintaxis highlight.
```

### Prompt: Code Review
```
Actúa como un senior code reviewer.

Revisa el siguiente código y proporciona feedback constructivo:

```[LENGUAJE]
[CÓDIGO A REVISAR]
```

Analiza y comenta sobre:

1. **Corrección**
   - ¿Funciona correctamente?
   - ¿Hay bugs potenciales?

2. **Best Practices**
   - ¿Sigue convenciones del lenguaje?
   - ¿Código limpio y legible?

3. **Performance**
   - ¿Hay optimizaciones posibles?
   - ¿Complejidad algorítmica adecuada?

4. **Seguridad**
   - ¿Vulnerabilidades potenciales?
   - ¿Validación de inputs?

5. **Mantenibilidad**
   - ¿Código fácil de mantener?
   - ¿Documentación suficiente?

6. **Sugerencias de Mejora**
   - Código refactorizado
   - Explicación de cambios

Usa este formato:
✅ Bien: [aspectos positivos]
⚠️ Mejorar: [áreas de mejora]
🔧 Refactor sugerido: [código mejorado]
```

---

## Categoría: Atención al Cliente

### Prompt: Respuesta a Queja de Cliente
```
Eres un especialista en customer success con alta empatía.

Un cliente ha presentado la siguiente queja:

[QUEJA DEL CLIENTE]

Contexto adicional:
- Tipo de cliente: [Nuevo/Recurrente/Premium]
- Producto/Servicio: [NOMBRE]
- Historial: [Breve contexto si es relevante]

Genera una respuesta que:
1. Reconozca el problema específicamente
2. Muestre empatía genuina
3. Explique qué salió mal (si se sabe)
4. Ofrezca solución concreta
5. Proponga compensación (si aplica)
6. Mencione pasos para prevenir futuro

Tono: Profesional, empático, orientado a solución
Longitud: 100-150 palabras
Incluye: Línea de cierre que invite a continuar conversación
```

### Prompt: Clasificación de Tickets
```
Clasifica el siguiente ticket de soporte:

Ticket:
[CONTENIDO DEL TICKET]

Proporciona:

1. **Categoría:**
   - [ ] Técnico
   - [ ] Facturación
   - [ ] Producto
   - [ ] Cuenta
   - [ ] Otro

2. **Prioridad:**
   - [ ] Crítica (servicio caído)
   - [ ] Alta (bloquea operación)
   - [ ] Media (afecta pero hay workaround)
   - [ ] Baja (pregunta general)

3. **Sentimiento:**
   - [ ] Molesto
   - [ ] Neutral
   - [ ] Satisfecho

4. **Departamento sugerido:**
   [Equipo técnico / Ventas / CS / etc.]

5. **Respuesta sugerida:** (50 palabras máximo)

6. **Requiere escalamiento:** [Sí/No] + justificación
```

---

## Categoría: Marketing

### Prompt: Generación de Copy para Ad
```
Crea copy para un anuncio de [PLATAFORMA: Facebook/Google/LinkedIn] sobre:

**Producto/Servicio:** [NOMBRE]
**Audiencia objetivo:** [PERFIL DETALLADO]
**Punto de dolor principal:** [PROBLEMA QUE RESUELVE]
**Beneficio clave:** [VALOR ÚNICO]
**CTA deseado:** [ACCIÓN]

Genera 3 variaciones de:

1. **Headline** (máx 40 caracteres)
2. **Body copy** (máx 125 caracteres)
3. **CTA button text** (máx 20 caracteres)

Para cada variación, explica:
- Enfoque psicológico usado
- Por qué debería funcionar con esta audiencia
- A/B test sugerido

Evita:
- Promesas no respaldadas
- Lenguaje generic
- Múltiples CTAs
```

---

## Categoría: Recursos Humanos

### Prompt: Descripción de Puesto
```
Crea una descripción de puesto atractiva y completa para:

**Posición:** [TÍTULO DEL PUESTO]
**Departamento:** [ÁREA]
**Reporta a:** [POSICIÓN]
**Ubicación:** [LUGAR/REMOTO]
**Tipo:** [Tiempo completo/Medio tiempo/Contrato]

Incluye:

1. **Resumen del Rol** (2-3 frases)
   - Misión principal
   - Impacto en la organización

2. **Responsabilidades Clave** (5-7)
   - Comienza con verbos de acción
   - Específicas y medibles

3. **Requisitos**
   - Educación
   - Experiencia (años y tipo)
   - Skills técnicos
   - Skills blandos

4. **Nice to Have** (3-4)

5. **Beneficios y Cultura** (4-5 puntos)
   - Beneficios tangibles
   - Oportunidades de crecimiento
   - Cultura de trabajo

6. **Proceso de Aplicación**

Tono: Inspirador pero profesional, inclusivo
Longitud: 400-500 palabras
```

---

## Técnicas Avanzadas

### Chain-of-Thought para Problemas Complejos
```
Resuelve el siguiente problema paso a paso, mostrando tu razonamiento:

Problema:
[DESCRIPCIÓN DETALLADA]

Por favor:
1. **Entiende el problema**
   - Reformula en tus palabras
   - Identifica componentes clave

2. **Descompón el problema**
   - Divide en sub-problemas
   - Lista dependencias

3. **Analiza cada sub-problema**
   - Opciones disponibles
   - Pros y contras

4. **Sintetiza la solución**
   - Combina insights
   - Propón approach integrado

5. **Valida**
   - ¿Resuelve el problema original?
   - ¿Hay edge cases no considerados?

6. **Recomendación final**
   - Acción concreta
   - Next steps
   - Riesgos y mitigaciones

Usa bullets, negritas y formato claro.
```

### Few-Shot Learning Template
```
Aprende del patrón en estos ejemplos y aplícalo al nuevo caso:

Ejemplo 1:
Input: [INPUT_1]
Output: [OUTPUT_1]
Explicación: [POR QUÉ]

Ejemplo 2:
Input: [INPUT_2]
Output: [OUTPUT_2]
Explicación: [POR QUÉ]

Ejemplo 3:
Input: [INPUT_3]
Output: [OUTPUT_3]
Explicación: [POR QUÉ]

Ahora aplica el mismo patrón a:
Input: [NUEVO_INPUT]
Output: [GENERA EL OUTPUT]
Explicación: [JUSTIFICA]
```

---

## Tips de Optimización

### Estructura Ganadora de Prompts
```
[ROL] + [CONTEXTO] + [TAREA] + [FORMATO] + [RESTRICCIONES] + [EJEMPLOS]

Ejemplo completo:
Eres un [ROL: especialista en X con Y años de experiencia].

Contexto: [SITUACIÓN, ANTECEDENTES, DATOS RELEVANTES]

Tarea: [QUÉ NECESITAS QUE HAGA, ESPECÍFICO]

Formato deseado:
- [ESTRUCTURA ESPERADA]
- [LONGITUD]
- [ESTILO/TONO]

Restricciones:
- [QUÉ NO HACER]
- [LIMITACIONES]
- [CONSIDERACIONES]

Ejemplos (opcional):
[SI APLICA, MUESTRA 1-2 EJEMPLOS DEL OUTPUT ESPERADO]
```

### Variables Reemplazables
En todos los prompts, reemplaza:
- `[TEXTO EN CORCHETES]` con tu información específica
- Ajusta longitudes según necesidad
- Modifica tono según audiencia
- Agrega restricciones específicas de tu contexto

### Iteración
1. Prueba el prompt
2. Evalúa resultado (1-10)
3. Identifica qué falta o sobra
4. Ajusta una variable a la vez
5. Re-prueba
6. Documenta qué funcionó

---

## Recursos Adicionales

**Librerías de prompts:**
- [PromptBase](https://promptbase.com)
- [ShareGPT](https://sharegpt.com)
- [Anthropic Prompt Library](https://docs.anthropic.com/claude/prompt-library)

**Testing:**
- OpenAI Playground
- Claude.ai
- Poe.com (múltiples modelos)

**Comunidades:**
- r/PromptEngineering
- Learn Prompting Discord
- AI Stack Devs Slack

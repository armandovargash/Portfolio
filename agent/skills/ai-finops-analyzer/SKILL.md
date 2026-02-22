# AI FinOps Analyzer (Unit Economics)

## 1. Description & Objective
Ejecuta simulaciones matemáticas y arquitectónicas para proyectar la viabilidad financiera (FinOps) de cualquier *feature* de Inteligencia Artificial propuesto. Frena inversiones de recursos ("De-Risking") si el *Time-to-Market* o el coste de inferencia rompen el margen.

## 2. Trigger (When to activate)
Actívalo **SIEMPRE** que el usuario pida: "Diseña esta feature con IA", "Añade ChatGPT/Claude a la plataforma", o proponga una idea de producto basada en LLMs (chatbots, generadores, agentes). 

## 3. Execution Rules & Validation Checklist (De-Risking)
**Execution Rules:**
- Tienes ESTRICTAMENTE PROHIBIDO empezar a escribir código para un feature de IA sin haber entregado primero la "Proyección FinOps".
- Debes entregar un reporte de 3 puntos:
  1. **Coste por Inferencia (Unit Economics):** Estima el gasto en Tópicos/Tokens. (Ej: "¿Cuánto cuesta usar GPT-4o para procesar 1,000 requests diarios?").
  2. **Análisis de Latencia (UX):** Calcula el TTFT (Time-To-First-Token) esperado. Frena la feature si la fricción supera 2 segundos en una UI *snappy*.
  3. **Veredicto Brutalista (Open Source vs Privado):** Recomienda modelos ligeros (Llama-3-8B, Mistral, Vertex) vs APIs cerradas si el margen asimétrico lo justifica.
- No uses adjetivos floridos. Usa tablas simples de markdown o viñetas cortas. Muestra las matemáticas claras.

**Validation Checklist (Binary Check before delivering to user):**
- [ ] ¿Entregaste el reporte con números reales o estimaciones razonables en lugar de simples promesas genéricas?
- [ ] ¿Calculaste el coste de la API por cada 1,000 interacciones de usuario?
- [ ] ¿Bloqueaste la ejecución del código hasta que el Founder aprobará explícitamente el P&L proyectado?
- [ ] ¿La salida está completamente libre de jerga corporativa hueca (cumpliendo `agent/rules/voz_armando.md`)?

## 4. Iteration & Feedback
Tras escupir el reporte FinOps, lanza siempre esta pregunta final:
*"El De-Risking está hecho. Las Unit Economics muestran [X gasto proyectado]. ¿Asumes el P&L y procedemos a inyectar el código, o pivotamos hacia un modelo Open-Source más barato?"*

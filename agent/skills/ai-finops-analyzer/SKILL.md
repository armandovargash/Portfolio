# Analizador FinOps de IA (Unit Economics)

## 1. Descripción y Objetivo
Ejecuta simulaciones matemáticas y arquitectónicas para proyectar la viabilidad financiera (FinOps) de cualquier funcionalidad de Inteligencia Artificial propuesta. Frena inversiones de recursos ("De-Risking") si el *Time-to-Market* o el coste de inferencia rompen el margen.

## 2. Disparador (Cuándo activar)
Actívalo **SIEMPRE** que el usuario pida: "Diseña esta funcionalidad con IA", "Añade ChatGPT/Claude a la plataforma", o proponga una idea de producto basada en LLMs (chatbots, generadores, agentes). 

## 3. Reglas de Ejecución y Checklist de Validación
**Reglas de Ejecución:**
- Tienes ESTRICTAMENTE PROHIBIDO empezar a escribir código para una feature de IA sin haber entregado primero la "Proyección FinOps".
- Debes entregar un reporte de 3 puntos:
  1. **Coste por Inferencia (Unit Economics):** Estima el gasto en Tópicos/Tokens. (Ej: "¿Cuánto cuesta usar GPT-4o para procesar 1,000 requests diarios?").
  2. **Análisis de Latencia (UX):** Calcula el TTFT (Time-To-First-Token) esperado. Frena la funcionalidad si la fricción supera 2 segundos en una interfaz rápida.
  3. **Veredicto Brutalista (Open Source vs Privado):** Recomienda modelos ligeros (Llama-3-8B, Mistral, Vertex) vs APIs cerradas si el margen asimétrico lo justifica.
- No uses adjetivos floridos. Usa tablas simples de markdown o viñetas cortas. Muestra las matemáticas claras.

**Checklist de Validación (Revisión binaria antes de entregar):**
- [ ] ¿Entregaste el reporte con números reales o estimaciones razonables en lugar de simples promesas genéricas?
- [ ] ¿Calculaste el coste de la API por cada 1,000 interacciones de usuario?
- [ ] ¿Bloqueaste la ejecución del código hasta que el Founder aprobara explícitamente el P&L proyectado?
- [ ] ¿La salida está completamente libre de jerga corporativa hueca (cumpliendo `agent/rules/voz_armando.md`)?

## 4. Iteración y Feedback
Tras entregar el reporte FinOps, lanza siempre esta pregunta final:
*"El De-Risking está hecho. Las Unit Economics muestran [X gasto proyectado]. ¿Asumes el P&L y procedemos a inyectar el código, o pivotamos hacia un modelo Open-Source más barato?"*

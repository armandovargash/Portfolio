# Validador de PRD (De-Risking de Producto)

## 1. Descripción y Objetivo
Evalúa los Documentos de Requisitos de Producto (PRDs) contra los estándares de Product Management, asegurando que se centren en FinOps de IA, validación rápida (Vibe Coding) y la regla del "3x ROI".

## 2. Disparador (Cuándo activar)
Actívalo siempre que el usuario proporcione un PRD, una idea de funcionalidad o un alcance de proyecto para revisión, o cuando pida "validar este concepto".

## 3. Reglas de Ejecución y Checklist de Validación
**Reglas de Ejecución:**
- SIEMPRE critica el documento basándote en la viabilidad del negocio y el "Time-to-Market", no solo en la completitud técnica de la funcionalidad.
- EXIGE evidencia de "Product Discovery". Si el PRD se basa en intuición sin datos o sin síntesis impulsada por agentes, señálalo inmediatamente.
- Haz cumplir la "Regla 3x": ¿La funcionalidad propuesta proyecta un valor (LTV/Retención) de al menos 3 veces el coste de su inferencia/cómputo de IA? Si no está definido, exígelo.
- Sugiere estrategias de "De-Risking": ¿Cómo se puede probar esto en días (ej. vía Vibe Coding) antes de comprometer recursos centrales de ingeniería?
- NO reescribas el PRD por completo a menos que se te pida; proporciona feedback quirúrgico y estratégico.

**Checklist de Validación (Revisión binaria antes de entregar):**
- [ ] ¿Evaluaste el PRD en términos de AI FinOps / Unit Economics?
- [ ] ¿Cuestionaste el proceso de descubrimiento (está respaldado por datos)?
- [ ] ¿Propusiste un método de prototipado más rápido para mitigar riesgos (De-Risking)?
- [ ] ¿El feedback mantiene el tono directo y realista exigido en `agent/rules/voz_armando.md`?

## 4. Iteración y Feedback
Una vez generado el análisis, pregunta al usuario:
*"Validación de PRD completada. He detectado los puntos de mayor fricción y riesgo. ¿Ajustamos el alcance para mejorar el Time-to-Market o ejecutamos este plan?"*

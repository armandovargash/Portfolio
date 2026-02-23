# Creador de Skills (Metaprogramación)

## 1. Descripción y Objetivo
Actúa como el ingeniero de sistemas del Senior Innovation PM. Genera nuevas habilidades estandarizadas para el agente, imponiendo la metodología Zero-to-One y de De-Risking.

## 2. Disparador (Cuándo activar)
Actívalo ÚNICAMENTE cuando el usuario pida explícitamente "crear una skill", "sistematizar un proceso" o "construir una nueva habilidad de agente".

## 3. Reglas de Ejecución y Checklist de Validación
**Reglas de Ejecución:**
- SIEMPRE crea una nueva carpeta para la habilidad solicitada usando la convención `kebab-case`.
- Dentro de esa nueva carpeta, SIEMPRE crea un archivo llamado exactamente `SKILL.md`.
- El archivo `SKILL.md` generado DEBE contener estrictamente las siguientes cuatro secciones en español:
    1. **Descripción y Objetivo:** Menos de 15 palabras definiendo qué hace y qué problema resuelve.
    2. **Disparador (Cuándo activar):** Contexto exacto de cuándo el agente debe activarla.
    3. **Reglas de Ejecución y Checklist de Validación:** Instrucciones paso a paso, restricciones estrictas (qué NO hacer) y criterios de revisión binarios (Sí/No).
    4. **Iteración y Feedback:** Una indicación final para ajustar el resultado.

**Checklist de Validación (Revisión binaria antes de entregar):**
- [ ] ¿Se creó una nueva carpeta con `kebab-case`?
- [ ] ¿El archivo principal se llama exactamente `SKILL.md`?
- [ ] ¿Contiene el `SKILL.md` las 4 secciones estructurales obligatorias en español?
- [ ] ¿La habilidad generada redacta sus instrucciones respetando la voz operativa de `agent/rules/voz_armando.md`?

## 4. Iteración y Feedback
Una vez generada y guardada la habilidad, pregunta al usuario: 
*"Esqueleto de la skill creado. Por favor, revisa el checklist de validación. ¿Hay alguna restricción estricta adicional que quieras añadir antes de bloquear esta habilidad para producción?"*
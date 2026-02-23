# Auditor de QA (Calidad Brutalista)

## 1. Descripción y Objetivo
Actúa como un ingeniero de Quality Assurance implacable. Obliga al agente a auditar proactivamente su propio trabajo (interfaz, código, consola, enlaces) antes de entregar cualquier resultado final al usuario.

## 2. Disparador (Cuándo activar)
Actívalo INMEDIATAMENTE antes de presentar cualquier código terminado, cambios de interfaz o nuevas funcionalidades al usuario.

## 3. Reglas de Ejecución y Checklist de Validación
**Reglas de Ejecución:**
- NUNCA asumas que el código funciona solo porque fue escrito. Debes verificarlo mediante simulación o una revisión propia rigurosa.
- SIEMPRE prueba la interfaz en múltiples tamaños de pantalla (estrictamente móvil y escritorio) buscando fallos de alineación, desbordamientos y roturas de diseño.
- SIEMPRE comprueba que no haya enlaces rotos ni dependencias fallidas (archivos CSS/JS faltantes, CDNs inaccesibles).
- SIEMPRE revisa la consola del navegador en busca de excepciones no controladas, advertencias o errores de red tras un cambio.
- Si encuentras un error, arréglalo proactivamente. No entregues código roto ni dependas del usuario para probarlo primero.

**Checklist de Validación (Revisión binaria antes de entregar):**
- [ ] ¿Verificaste la adaptabilidad estricta (móvil y escritorio)?
- [ ] ¿Confirmaste que NO hay errores ni advertencias en la consola?
- [ ] ¿Todos los enlaces son funcionales y las dependencias cargan correctamente?
- [ ] Evaluación de Interfaz Brutalista: ¿El fondo es estrictamente #000000 con CERO propiedades de `box-shadow` o `drop-shadow`?
- [ ] Evaluación de Arquitectura Zero-Debt: ¿La implementación es puramente HTML Semántico, Tailwind CSS y Vanilla JS, sin introducir frameworks pesados (como React) ni procesos de compilación?
- [ ] Evaluación de Integración en Vivo: ¿Todos los iframes inyectados (ej. Scratch) y enlaces externos resuelven correctamente sin causar errores de origen cruzado (cross-origin) o en consola?
- [ ] ¿El feedback del auditor mantiene el tono directo y "ex-founder" de `agent/rules/voz_armando.md`?

## 4. Iteración y Feedback
Tras completar la auditoría, presenta el resultado y pregunta:
*"Auditoría completada. Todo el código y la interfaz pasaron el filtro. ¿Desplegamos a producción o quieres que le demos otra vuelta?"*

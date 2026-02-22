# FORMATOS DE SALIDA ESTRICTOS Y EJEMPLOS (FEW-SHOT)

Para garantizar un comportamiento predecible y determinista (Best Practice de Google AI Studio), el agente debe estructurar sus respuestas usando estos patrones.

## 1. Patrón de Redacción Directa (Copywriting)
Cuando el usuario pida iterar texto, el agente NO debe usar introducciones robóticas como "Claro, aquí tienes una opción". Debe entregar la salida cruda.

**Ejemplo de Transacción:**
*[Input del Usuario:]* "Cámbiale el texto a este botón que dice 'Contáctame' por algo más de negocios."
*[Output del Agente:]* `[ Ejecutar Reunión Táctica ]`

## 2. Patrón de Auditoría y Reporte de Bugs
Cuando se solicite examinar código o una UI, la respuesta debe estructurarse obligatoriamente bajo estos 3 encabezados:

1. **DIAGNÓSTICO:** [Explicación técnica en 1 línea del problema o éxito]
2. **IMPACTO (De-Risking):** [Por qué esto importa a nivel UX, negocio o estética Brutalista]
3. **ACCIÓN TÁCTICA:** [Qué líneas de código se van a destruir/inyectar para solucionarlo]

## 3. Patrón de Solicitud de Permiso (Git/Vercel)
Cuando el agente necesite hacer `git push` a producción, siempre debe finalizar su mensaje con una pregunta de confirmación binaria explícita.
*Ejemplo:* "¿Tienes luz verde para compilar este commit en la rama main y disparar Vercel?"

# LÍMITES OPERATIVOS Y SEGURIDAD (BOUNDARIES)

Este documento define la "Caja de Arena" (Sandbox) técnica y de comportamiento del agente IA. Estas son reglas restrictivas absolutas.

## 1. Límites Tecnológicos (Tech Stack)
- **Bloqueo de Frameworks:** Tienes estrictamente prohibido sugerir o ejecutar migraciones a React, Vue, Next.js, Svelte, o introducir bundlers (Webpack/Vite). El portafolio vive en **Vanilla JS + HTML + Tailwind CDN**. 
- **Librerías Externas:** Cero importaciones de CDNs adicionales sin orden explícita (Prohibido traer jQuery, Bootstrap, o librerías de animaciones masivas como GSAP a menos que el usuario lo exija para un MVP).

## 2. Protocolo Anti-Alucinación (Incertidumbre)
- **Métricas:** Si estás redactando un caso de estudio y faltan KPIs, NO inventes números. Usa corchetes de bloqueo: `[INSERTAR KPI]` o detén la ejecución pidiendo el dato al usuario.
- **Funcionalidad Mágica:** Si el usuario pide algo que requiere backend (ej. una base de datos real en este HTML estático), advierte inmediatamente de la limitación arquitectónica.

## 3. Comportamiento en Resolución de Errores
- **Cero Disculpas Robóticas:** Si te equivocas al programar, nunca digas "Lo siento, tienes razón, me equivoqué". Simplemente di: "Error detectado en X. Inyectando parche inmediato." Resuelve y avanza.
- **Protección de Código:** Cuando modifiques archivos HTML/CSS, prioriza alterar solo el bloque en cuestión. Evita reescribir archivos enteros desde cero si ya hay arquitectura validada.

# ARQUITECTURA TÉCNICA DEL PORTAFOLIO: DE CERO A UNO

## 1. Stack Tecnológico (Restricciones Base)
- **Estructura:** HTML5 Semántico.
- **Estilos:** Tailwind CSS (cargado obligatoriamente vía CDN) y CSS Vanilla.
- **Lógica:** Vanilla JavaScript puro. Prohibido el uso de frameworks pesados para garantizar un código rápido y ligero.
- **Tipografía:** Google Fonts (Inter).

## 2. Estructura Estricta de Archivos (3 Archivos Máximo)
### A. index.html (Esqueleto Semántico)
Debe contener estrictamente estos bloques en orden:
1. `<div id="preloader">`: Pantalla negra con texto centrado para la entrada cinemática.
2. `<header id="main-header">`: Cabecera superior fija con efecto de cristal (glassmorphism oscuro).
3. `<section id="inicio">`: Contenedor alineado a la izquierda con un texto `<h1>` inmenso (7.5rem).
4. `<section id="proyectos">`: Cuadrícula asimétrica (Bento Grid). Contiene botones/artículos con métricas abstractas de fondo y clases base como `bg-darkCard`.
5. `<div id="cmd-modal">`: Modal oscuro (overlay) estilo Spotlight para el menú de comandos (atajo ⌘K).
6. `<div id="project-modal">`: Modal instantáneo estructurado en: Contexto, Ejecución y Tech Stack para detallar los proyectos.

### B. style.css (Solo CSS Crítico)
Exclusivo para la lógica que Tailwind no cubre nativamente vía CDN:
- `::-webkit-scrollbar`: Barra de desplazamiento premium oscura y estilizada.
- `input:-webkit-autofill`: Reseteo de estilos nativos del navegador paraInputs en modo oscuro.
- **Animaciones:** Coreografía de entrada `@keyframes fadeInUp`.
- **Comando K:** Estilos para la barra de scroll miniatura dentro del menú de comandos (`.custom-scrollbar`).

### C. script.js (El Cerebro)
Lógica modularizada dentro de un `DOMContentLoaded`. Contiene:
- **Preloader:** Temporizador orquestado para desvanecer la pantalla negra y liberar el scroll.
- **Command Menu (⌘K):** Lógica para abrir/cerrar escuchando `Cmd + K` o `Ctrl + K`, permitir navegación con flechas (Up/Down) y filtrado de texto rápido.
- **Modales de Proyecto:** Un objeto JSON interno `projectData` que almacena la información de los *Case Studies* para inyectarla dinámicamente en el modal sin recargar la página.

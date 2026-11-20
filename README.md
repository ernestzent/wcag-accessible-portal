# A11y Web Studio - Portal Web Accesible (WCAG 2.1 AA) ♿

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![WCAG 2.1 AA](https://img.shields.io/badge/WCAG_2.1-Level_AA-success?style=for-the-badge)
![WAI-ARIA](https://img.shields.io/badge/WAI--ARIA-Compliant-blue?style=for-the-badge)

¡Hola! 👋 **A11y Web Studio** es un portal web multipágina desarrollado bajo un estricto cumplimiento de los estándares de accesibilidad **WCAG 2.1 Nivel AA**. El proyecto está enfocado en demostrar prácticas sólidas de ingeniería web inclusiva para personas que navegan mediante teclado, lectores de pantalla o ajustes de alto contraste.

🔗 **Demo en vivo:** [Ver A11y Web Studio desplegado](https://wcag-accessible-portal.netlify.app/)

## ✨ Características Principales

* **Arquitectura HTML5 Semántica:** Uso correcto de *landmarks* (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`), jerarquía lógica de encabezados y estructura pensada para tecnologías de asistencia en `index.html` y `contacto.html`.
* **Roles y Atributos WAI-ARIA:** Implementación precisa de atributos como `aria-current="page"`, `aria-label`, `aria-describedby` y regiones accesibles para mejorar la experiencia con lectores de pantalla.
* **Navegación Completa por Teclado:** Orden de tabulación predecible sin trampas de foco, permitiendo recorrer enlaces, botones y campos de formulario exclusivamente con el teclado.
* **Indicadores `:focus-visible` de Alto Contraste:** Contornos claros y visibles en `styles.css` al navegar con `Tab`, acompañados de relaciones de contraste conformes a WCAG 2.1 AA y soporte para zoom del navegador sin pérdida de legibilidad.

## 🛠️ Tecnologías Utilizadas

* **HTML5 Semántico:** Maquetación multipágina accesible (`index.html`, `contacto.html`).
* **CSS3:** Estilos de alto contraste, indicadores `:focus-visible` y diseño responsivo (`styles.css`).
* **Estándares y Auditoría:** WCAG 2.1 Nivel AA, WAI-ARIA, Google Lighthouse (Accessibility) y verificación con herramientas de accesibilidad.

## 📂 Estructura del Proyecto

```text
wcag-accessible-portal/
├── contacto.html               # Página de contacto con formulario accesible y atributos ARIA
├── index.html                  # Página principal con landmarks semánticos y navegación accesible
├── styles.css                  # Hoja de estilos con alto contraste e indicadores :focus-visible
```

## 🚀 Instalación y Uso

Al ser un proyecto estático construido con HTML5 y CSS3 nativos, no requiere instalación de dependencias ni compilación:

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/ernestzent/wcag-accessible-portal.git
   cd wcag-accessible-portal
   ```

2. **Abre el proyecto:**
   * Haz doble clic en `index.html` para visualizarlo directamente en tu navegador, **o**
   * Ejecútalo con la extensión **Live Server** de VS Code para probar la navegación entre páginas con recarga automática.

## 💡 Ejemplos de Uso

1. **Navegación Exclusiva por Teclado:** Abre `index.html` y utiliza únicamente **`Tab`**, **`Shift + Tab`** y **`Enter`** para recorrer el menú, verificar los indicadores `:focus-visible` y desplazarte hacia `contacto.html`.
2. **Prueba de Formulario Accesible:** En `contacto.html`, navega por cada campo con el teclado para comprobar la asociación entre etiquetas (`<label>`) e inputs, así como las indicaciones accesibles.
3. **Prueba de Zoom y Contraste:** Aumenta el zoom del navegador hasta el **200%** para validar que el contenido se reacomoda limpiamente sin generar desplazamiento horizontal.

## 🤝 Contribuciones

Toda contribución orientada a mejorar la compatibilidad con lectores de pantalla o estándares WCAG es bienvenida:
1. Haz un *Fork* del repositorio.
2. Crea tu rama (`git checkout -b a11y/mejora-aria`).
3. Guarda tus cambios (`git commit -m 'Mejora atributos ARIA en formulario de contacto'`).
4. Sube tu rama (`git push origin a11y/mejora-aria`).
5. Abre un *Pull Request* indicando qué herramienta o lector de pantalla utilizaste para validarlo.

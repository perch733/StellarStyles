# StellarStyles.css

**StellarStyles.css** es la alternativa definitiva a `normalize.css`, diseñada para ofrecerte una base sólida y moderna para tus proyectos CSS. Con **StellarStyles**, obtienes una normalización del estilo en todos los navegadores, mejorando la consistencia y la compatibilidad de tus diseños web.

**StellarStyles.css** is the ultimate alternative to `normalize.css`, designed to provide a modern, solid foundation for your CSS projects. With **StellarStyles**, you get consistent style normalization across all browsers, improving both design consistency and cross-browser compatibility.

## ¿Por qué elegir StellarStyles.css? / Why Choose StellarStyles.css?

- **Sólida Alternativa a Normalize.css**: Mientras que `normalize.css` se enfoca en igualar el estilo de los elementos básicos, **StellarStyles** lleva esto un paso más allá, proporcionando una solución más completa y moderna para las diferencias entre navegadores.
- **A Strong Alternative to Normalize.css**: While normalize.css focuses on equalizing basic element styles, StellarStyles takes it a step further — offering a more complete and modern solution for browser inconsistencies.
- **Estilos Modernos y Mejorados**: Con una base cuidadosamente diseñada, **StellarStyles** corrige problemas comunes de diseño y proporciona estilos optimizados que funcionan en todos los navegadores más populares.
- **Modern and Enhanced Styling**: Carefully crafted, **StellarStyles** fixes common design issues and provides optimized styles that work seamlessly across all major browsers.
- **Optimización para la Mayor Compatibilidad**: **StellarStyles** asegura que tu sitio se vea bien en los navegadores más utilizados, proporcionando soporte extendido mientras elimina incompatibilidades innecesarias.
- **Optimized for Maximum Compatibility: StellarStyles** ensures your site looks great in the most popular browsers, providing extended support while removing unnecessary inconsistencies.
- **Configuración Sencilla**: Fácil de integrar y configurar, **StellarStyles** se adapta perfectamente a tus necesidades sin complicaciones. Solo tienes que incluirlo en tu proyecto y listo.
- **Simple Setup**: Easy to integrate and configure, **StellarStyles** adapts effortlessly to your workflow — just include it in your project and you’re ready to go.
- **Mantenimiento Activo y Soporte**: Manteniéndote al día con las últimas tendencias y estándares web, **StellarStyles** asegura que tu proyecto esté siempre en la vanguardia de la compatibilidad CSS.
- **Active Maintenance and Support**: Stay aligned with the latest web standards and trends. StellarStyles keeps your project on the cutting edge of CSS compatibility.

## Instalación / Installation

Para empezar a usar **StellarStyles.css** en tu proyecto, sigue estos pasos: / To start using StellarStyles.css in your project, follow these steps:

1. **Instala la librería**: / **Install the library**:

   ```bash
   npm install stellarstyles.css
   ```

2. **Incluye el CSS en tu proyecto**: / **Include the CSS in your project**:

   En tu archivo principal CSS o JS: / In your main CSS or JS file:

   ```js
   import "stellarstyles.css";
   ```

## Características / Features

- **Box-sizing:** Ajusta el box-sizing para una mejor consistencia / Adjusts the box-sizing model for consistent layout behavior.
- **Tipografía y Fuentes:** Corrección de fuentes y tamaños de manera uniforme / Ensures uniform font sizing and rendering.
- **Estilos de Formularios:** Mejora en la apariencia y comportamiento de formularios / Improves the appearance and usability of form elements.
- **Compatibilidad con Selecciones:** Estilo consistente para selecciones de texto / Provides consistent styling for text selections.
- **Soporte Extendido:** Compatible con la mayoría de navegadores y dispositivos / Fully compatible across modern browsers and devices.

## Compatibilidad con Encabezados `<h1>` Anidados

### 🔔 Actualización importante sobre los estilos por defecto de `<h1>` / Important update about default `<h1>` styles

A partir de 2025, los navegadores están eliminando los estilos por defecto que reducían visualmente los tamaños de los encabezados `<h1>` anidados dentro de elementos como `<section>`, `<article>`, `<nav>` y `<aside>` / Starting in 2025, browsers are removing the default styles that visually reduced the size of `<h1>` headings nested inside elements like `<section>`, `<article>`, `<nav>` y `<aside>`.

Para más detalles sobre los cambios visita la [El siguiente Blog en Mozilla](https://developer.mozilla.org/en-US/blog/h1-element-styles/). / For more details, visit the [official Mozilla blog](https://developer.mozilla.org/en-US/blog/h1-element-styles/).

Esto puede provocar advertencias en herramientas como Lighthouse si no se define un tamaño de fuente explícito para cada `<h1>` / This change may trigger warnings in tools like Lighthouse if you don’t define an explicit font size for each `<h1>`.

**StellarStyles.css** ya aplica un estilo uniforme explícito para todos los `<h1>`, cumpliendo con las nuevas recomendaciones: / already applies a consistent explicit style for all `<h1>` elements, following the new recommendations.

```css
:where(h1) {
  font-size: 2em;
  margin-block: 0.67em;
}
```

## Selección y subrayado / Selection and Underline Control

Si deseas importar únicamente el estilo de selección de texto o subrayado controlado, puedes hacerlo fácilmente: / If you want to import only the text selection and underline control styles, you can easily do so:

```js
import "stellarstyles.css/selection";
```

> 📘 Nota: Este módulo aplica estilos consistentes para ::selection y control de subrayado, mejorando la accesibilidad visual del texto seleccionado.

> 📘 Note: This module provides consistent ::selection and underline control styles, improving text accessibility and visual clarity.

## Documentación / Documentation

Para más detalles sobre las características y el uso de **StellarStyles.css**, visita la [documentación completa](https://stellarstyles-css.percychuzon.com/) / For full details on StellarStyles.css features and usage, visit the [complete documentation](https://stellarstyles-css.percychuzon.com/).

## Contribuciones / Contributing

Si deseas contribuir a **StellarStyles.css**, por favor revisa nuestras [guías de contribución](https://github.com/perch733/StellarStyles/issues). Estamos abiertos a sugerencias y mejoras. / If you’d like to contribute to StellarStyles.css, please review our [contribution guidelines](https://github.com/perch733/StellarStyles/issues). We welcome suggestions and improvements!

## Soporte / Support

Para reportar problemas o hacer preguntas, por favor abre un [issue en GitHub](https://github.com/perch733/StellarStyles/issues). / To report issues or ask questions, please open an [issue on GitHub](https://github.com/perch733/StellarStyles/issues).

## Licencia / License

**StellarStyles.css** se distribuye bajo la licencia MIT. / **StellarStyles.css** is distributed under the MIT License.

Inspirado en [Normalize.css](https://github.com/necolas/normalize.css) y [Modern Normalize](https://github.com/sindresorhus/modern-normalize). / Inspired by [Normalize.css](https://github.com/necolas/normalize.css) and [Modern Normalize](https://github.com/sindresorhus/modern-normalize).

# StellarStyles.css

**StellarStyles.css** es la alternativa definitiva a `normalize.css`, diseñada para ofrecerte una base sólida y moderna para tus proyectos CSS. Con **StellarStyles**, obtienes una normalización del estilo en todos los navegadores, mejorando la consistencia y la compatibilidad de tus diseños web.

## ¿Por qué elegir StellarStyles.css?

- **Sólida Alternativa a Normalize.css**: Mientras que `normalize.css` se enfoca en igualar el estilo de los elementos básicos, **StellarStyles** lleva esto un paso más allá, proporcionando una solución más completa y moderna para las diferencias entre navegadores.
- **Estilos Modernos y Mejorados**: Con una base cuidadosamente diseñada, **StellarStyles** corrige problemas comunes de diseño y proporciona estilos optimizados que funcionan en todos los navegadores más populares.
- **Optimización para la Mayor Compatibilidad**: **StellarStyles** asegura que tu sitio se vea bien en los navegadores más utilizados, proporcionando soporte extendido mientras elimina incompatibilidades innecesarias.
- **Configuración Sencilla**: Fácil de integrar y configurar, **StellarStyles** se adapta perfectamente a tus necesidades sin complicaciones. Solo tienes que incluirlo en tu proyecto y listo.
- **Mantenimiento Activo y Soporte**: Manteniéndote al día con las últimas tendencias y estándares web, **StellarStyles** asegura que tu proyecto esté siempre en la vanguardia de la compatibilidad CSS.

## Instalación

Para empezar a usar **StellarStyles.css** en tu proyecto, sigue estos pasos:

1. **Instala la librería**:

   ```bash
   npm install stellarstyles.css
   ```

2. **Incluye el CSS en tu proyecto**:

   En tu archivo principal CSS o JS:

   ```js
   import "stellarstyles.css";
   ```

## Características

- **Box-sizing:** Ajusta el box-sizing para una mejor consistencia.
- **Tipografía y Fuentes:** Corrección de fuentes y tamaños de manera uniforme.
- **Estilos de Formularios:** Mejora en la apariencia y comportamiento de formularios.
- **Compatibilidad con Selecciones:** Estilo consistente para selecciones de texto.
- **Soporte Extendido:** Compatible con la mayoría de navegadores y dispositivos.

## Compatibilidad con Encabezados `<h1>` Anidados

### 🔔 Actualización importante sobre los estilos por defecto de `<h1>`

A partir de 2025, los navegadores están eliminando los estilos por defecto que reducían visualmente los tamaños de los encabezados `<h1>` anidados dentro de elementos como `<section>`, `<article>`, `<nav>` y `<aside>`.

Esto puede provocar advertencias en herramientas como Lighthouse si no se define un tamaño de fuente explícito para cada `<h1>`.

**StellarStyles.css** ya aplica un estilo uniforme explícito para todos los `<h1>`, cumpliendo con las nuevas recomendaciones:

```css
:where(h1) {
  font-size: 2em;
  margin-block: 0.67em;
}
```

### 🧩 ¿Necesitas replicar el estilo jerárquico antiguo?

Si prefieres simular el comportamiento visual anterior (donde los `<h1>` se veían como `<h2>`, `<h3>`, etc. al anidarse), puedes agregar este bloque manualmente en tu propio CSS:

```css
section h1 {
  font-size: 1.5em;
  margin-block: 0.83em;
}
section section h1 {
  font-size: 1.17em;
  margin-block: 1em;
}
section section section h1 {
  font-size: 1em;
  margin-block: 1.33em;
}
section section section section h1 {
  font-size: 0.83em;
  margin-block: 1.67em;
}
section section section section section h1 {
  font-size: 0.67em;
  margin-block: 2.33em;
}
```

> ⚠️ **Recomendación**: Para mantener una semántica correcta y evitar problemas de accesibilidad, utiliza etiquetas `<h2>`, `<h3>`, etc., en lugar de múltiples `<h1>` anidados.

---

### 🧩 Estilos heredados con archivo adicional (opcional)

También puedes importar un archivo CSS adicional que incluye este comportamiento jerárquico clásico directamente desde el mismo paquete:

```js
import "stellarstyles.css/h1-legacy";
```

Este archivo no se aplica por defecto. Solo se incluirá si lo importas explícitamente. Aplica estilos visuales progresivos a los encabezados `<h1>` anidados dentro de elementos como `<section>` o `<article>`, simulando la jerarquía de los antiguos estilos UA (User-Agent).

> Recomendado únicamente si trabajas con contenido heredado o necesitas mantener una jerarquía visual clásica por razones específicas.

### ✅ Beneficios

- **Separación clara de responsabilidades:** el archivo principal es moderno; el archivo alternativo es opcional.
- **Evita sorpresas para quienes no lo necesitan.**
- **Fácil de mantener:** si los navegadores cambian algo más, puedes actualizar `stellarstyles-h1-legacy.css` sin tocar el núcleo.

## Documentación

Para más detalles sobre las características y el uso de **StellarStyles.css**, visita la [documentación completa](https://stellarstyles-css.percychuzon.com/).

## Contribuciones

Si deseas contribuir a **StellarStyles.css**, por favor revisa nuestras [guías de contribución](https://imagelazy.percychuzon.com/). Estamos abiertos a sugerencias y mejoras.

## Soporte

Para reportar problemas o hacer preguntas, por favor abre un [issue en GitHub](https://github.com/perch33/StellarStyles/issues).

## Licencia

**StellarStyles.css** se distribuye bajo la licencia ISC.

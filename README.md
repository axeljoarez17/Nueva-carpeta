# Currículum en HTML puro

Mi currículum como página web, construido solo con HTML semántico y accesible, sin CSS ni JavaScript.

**Ver en vivo:** https://axeljoarez17.github.io/curriculum/

Es el proyecto de salida de la Fase 1 de mi ruta para convertirme en desarrollador web.

## Qué incluye

- Perfil, educación, habilidades, idiomas, proyectos y contacto.
- Un menú con enlaces a cada sección.
- Un enlace "Ir al contenido" para quien navega con teclado.

## Decisiones de HTML

| Elemento | Dónde lo usé | Por qué |
|---|---|---|
| `header`, `main`, `footer` | Estructura de la página | Un lector de pantalla los anuncia como regiones, y el usuario puede saltar directo al contenido. |
| `h1` con mi nombre | Cabecera | En un currículum, lo más importante de la página es la persona. |
| `section` con `h2` e `id` | Cada parte del CV | Cada sección tiene título para poder encontrarla navegando por títulos, y un `id` para el menú. |
| `article` con `h3` | Educación | Cada carrera es un bloque completo que tiene sentido por sí solo. |
| `time` con `datetime` | Periodos de estudio | La persona lee "Agosto 2026" y las máquinas leen `2026-08`. |
| `dl`, `dt`, `dd` | Idiomas | Son pares de nombre y valor: idioma → nivel. |
| `abbr` | Siglas | Explica qué significa una sigla la primera vez que aparece. |
| `address` | Contacto | Agrupa la información de contacto del autor de la página. |

## Accesibilidad

- Una sola jerarquía de títulos: `h1` → `h2` → `h3`, sin saltos.
- Todos los enlaces dicen a dónde llevan; ninguno abre otra pestaña sin avisar.
- La página se puede recorrer completa con la tecla Tab.
- `lang="es"` para que los lectores de pantalla pronuncien en español.

## Validación

- Validador del W3C: 0 errores.
- WAVE: 0 errores.

## Uso de IA

Escribí el código HTML yo mismo. Usé a Claude (Anthropic) como mentor para revisar cada versión del código y explicarme los errores. El texto del perfil, la lista de habilidades y las descripciones de los proyectos los redacté con ayuda de Claude y los adapté a mi situación.

## Qué aprendí

- A planear la estructura de títulos antes de escribir código.
- A usar `time` y `abbr`, dos etiquetas que no conocía.
- A validar cada sección al terminarla en lugar de esperar al final.

## Siguiente paso

En la Fase 2 le daré diseño con CSS, sin cambiar la estructura de HTML.
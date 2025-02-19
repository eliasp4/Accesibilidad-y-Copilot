# Proyecto de Accesibilidad Web WCAG 2.2

## Descripción

Este proyecto tiene como objetivo desarrollar un prompt efectivo para asistentes de programación inteligentes, como GitHub Copilot, que permita modificar código HTML para cumplir con los estándares de accesibilidad web establecidos por la normativa WCAG 2.2 (WAI). Se ha validado la eficacia del prompt utilizando diversas herramientas de validación de accesibilidad, garantizando el cumplimiento de los criterios A, AA y AAA.

## Objetivos

- Desarrollar un prompt claro, conciso y efectivo para la mejora de la accesibilidad web.
- Asegurar que el código HTML modificado cumpla con los criterios de accesibilidad WCAG 2.2 (A, AA y AAA).
- Documentar el proceso de desarrollo, validación y solución de problemas.

## Proceso de Desarrollo

1.  **Creación de Archivos HTML de Ejemplo:**
    -   Se crearon cuatro archivos HTML (`index1.html`, `index2.html`, `index3.html`, `index4.html`) con diferentes estructuras y elementos para representar diversos escenarios web. El `index4.html` fue diseñado como el caso más complejo.

2.  **Desarrollo del Prompt Inicial:**
    -   Se redactó un prompt inicial basado en los requisitos de accesibilidad WCAG 2.2.

3.  **Aplicación del Prompt:**
    -   El prompt fue aplicado a cada archivo HTML utilizando asistentes de programación de IA (ChatGPT y Perplexity).
    -   Se revisaron y adaptaron las modificaciones generadas por la IA para asegurar la correcta implementación de las mejoras de accesibilidad.

4.  **Validación de la Accesibilidad:**
    -   Se utilizaron las siguientes herramientas de validación de accesibilidad:
        -   WAVE (Web Accessibility Evaluation Tool)
        -   Axe (Accessibility Testing Tool)
        -   Lighthouse (Google Chrome)

5.  **Iteración y Refinamiento:**
    -   Se analizaron los resultados de las herramientas de validación y se identificaron los problemas de accesibilidad restantes.
    -   Se ajustó el prompt y se volvieron a aplicar las modificaciones hasta lograr un código accesible.

## Prompt Final

Modifica el siguiente código HTML para cumplir con los estándares de accesibilidad web
WCAG 2.2 (WAI) nivel AA y AAA. Realiza las siguientes acciones:
1. Añade atributos ARIA apropiados a todos los elementos interactivos (formularios,
botones, enlaces).
2. Mejora la semántica utilizando etiquetas HTML5 como <header>, <main>, <nav>,
<footer>, <section>, y <article>.
3. Asegúrate de que todas las imágenes tengan textos alternativos descriptivos y
significativos.
4. Verifica y corrige la estructura de encabezados [(<h1> a <h6>)] para que sea
jerárquicamente correcta.
5. Implementa una navegación por teclado lógica y accesible.
6. Asegura un contraste de color adecuado entre el texto y el fondo (relación mínima de
4.5:1 para AA, 7:1 para AAA).
7. Añade etiquetas descriptivas a todos los campos de formulario.
8. Incluye instrucciones claras para los campos de formulario que requieran un formato
específico.
9. Asegúrate de que todos los elementos interactivos tengan un área de interacción
mínima de 44x44 píxeles.
10. Implementa un skip link al inicio de la página para saltar directamente al contenido
principal.
11. Asegúrate de que el idioma de la página esté correctamente especificado.
12. Proporciona subtítulos y transcripciones para contenido multimedia si es aplicable.
13. Evita el uso de atributos que dependan únicamente del color para transmitir información.
14. Asegúrate de que el contenido sea legible y funcional cuando se amplía hasta un 200%.
15. Verifica que todos los atributos aria-labelledby y aria-describedby referencien un id
existente en la página.
16. Asegura que los elementos referenciados por aria-labelledby y aria-describedby
contengan etiquetas o descripciones adecuadas.
17. Si la página no tiene un <h1>, agrégalo con un título claro y descriptivo.
18. Asegura que la jerarquía de encabezados sea coherente (<h1> → <h2> → <h3>, etc.).
19. Para <video> con audio, asegúrate de incluir subtítulos sincronizados (<track> con
kind="captions").
20. Para <audio> y <video>, proporciona una transcripción accesible en texto.
21. Verifica que el contenido multimedia tenga una alternativa textual adecuada para
usuarios con discapacidades auditivas.
Aplica estas modificaciones manteniendo la funcionalidad original del código. Comenta cada
cambio significativo para explicar su propósito en relación con la accesibilidad.

## Herramientas Utilizadas

-   Asistentes de Programación de IA: ChatGPT, Perplexity
-   Herramientas de Validación de Accesibilidad:
    -   WAVE (Web Accessibility Evaluation Tool)
    -   Axe (Accessibility Testing Tool)
    -   Lighthouse (Google Chrome)

## Problemas Encontrados y Soluciones

| Problema                               | Solución Aplicada                                                                                                                                      |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Falta de estructura semántica          | Implementación de etiquetas HTML5 semánticas (`<header>`, `<main>`, `<nav>`, `<footer>`).                                                                   |
| Imágenes sin texto alternativo         | Adición de atributos `alt` descriptivos a todas las imágenes.                                                                                             |
| Formularios sin etiquetas asociadas    | Agregación de elementos `<label>` y asociación correcta con los campos de formulario mediante el atributo `for`.                                             |
| Contraste de color insuficiente       | Ajuste de colores del texto y fondo para cumplir con las relaciones de contraste requeridas (mínimo 4.5:1 para AA, 7:1 para AAA).                           |
| Falta de encabezados jerárquicos      | Reestructuración de los encabezados para seguir una jerarquía lógica desde `<h1>` hasta `<h6>`.                                                               |
| Elementos interactivos sin ARIA        | Añadido roles ARIA y atributos `aria-label` y `aria-describedby` para mejorar la accesibilidad de elementos interactivos.                                   |
| Contenido multimedia no accesible     | Inclusión de subtítulos para videos y transcripciones para audios.                                                                                         |
| Atributos ARIA con referencias rotas | Verificación y corrección de referencias en atributos `aria-labelledby` y `aria-describedby` para asegurar que apuntan a elementos existentes y descriptivos. |

## Resultados de la Validación

A continuación, se presentan los resultados de las herramientas de validación antes y después de aplicar el prompt y realizar las correcciones.

### index1.html

-   Accesibilidad antes: [Captura de pantalla: Accesibilidad antes index1]
-   Accesibilidad después: [Captura de pantalla: Accesibilidad después index1\_accesible]

### index2.html

-   Accesibilidad antes: [Captura de pantalla: Accesibilidad antes index2]
-   Accesibilidad después: [Captura de pantalla: Accesibilidad después index2\_accesible]

### index3.html

-   Accesibilidad antes: [Captura de pantalla: Accesibilidad antes index3]
-   Accesibilidad después: [Captura de pantalla: Accesibilidad después index3\_accesible]

### index4.html

-   Accesibilidad antes: [Captura de pantalla: Accesibilidad antes index4]
-   Accesibilidad después: [Captura de pantalla: Accesibilidad después index4\_accesible]

## Conclusiones

El prompt desarrollado demostró ser altamente efectivo para mejorar la accesibilidad de los archivos HTML, incluso en el caso más complejo del `index4.html`. La combinación del prompt, los asistentes de IA y las herramientas de validación permitió identificar y solucionar una amplia gama de problemas de accesibilidad, cumpliendo con los criterios WCAG 2.2 A, AA y AAA.

---

## English Version

# WCAG 2.2 Web Accessibility Project

## Description

This project aims to develop an effective prompt for intelligent programming assistants, such as GitHub Copilot, to modify HTML code to comply with web accessibility standards set by WCAG 2.2 (WAI). The effectiveness of the prompt has been validated using various accessibility validation tools, ensuring compliance with criteria A, AA, and AAA.

## Objectives

- Develop a clear, concise, and effective prompt for improving web accessibility.
- Ensure that the modified HTML code complies with WCAG 2.2 accessibility criteria (A, AA, and AAA).
- Document the development, validation, and troubleshooting process.

## Development Process

1.  **Creation of Sample HTML Files:**
    -   Four HTML files (`index1.html`, `index2.html`, `index3.html`, `index4.html`) were created with different structures and elements to represent various web scenarios. `index4.html` was designed as the most complex case.

2.  **Development of the Initial Prompt:**
    -   An initial prompt was drafted based on WCAG 2.2 accessibility requirements.

3.  **Application of the Prompt:**
    -   The prompt was applied to each HTML file using AI programming assistants (ChatGPT and Perplexity).
    -   The modifications generated by the AI were reviewed and adapted to ensure the correct implementation of accessibility improvements.

4.  **Accessibility Validation:**
    -   The following accessibility validation tools were used:
        -   WAVE (Web Accessibility Evaluation Tool)
        -   Axe (Accessibility Testing Tool)
        -   Lighthouse (Google Chrome)

5.  **Iteration and Refinement:**
    -   The results of the validation tools were analyzed, and remaining accessibility issues were identified.
    -   The prompt was adjusted, and modifications were reapplied until accessible code was achieved.

## Final Prompt

Modifica el siguiente código HTML para cumplir con los estándares de accesibilidad web
WCAG 2.2 (WAI) nivel AA y AAA. Realiza las siguientes acciones:
1. Añade atributos ARIA apropiados a todos los elementos interactivos (formularios,
botones, enlaces).
2. Mejora la semántica utilizando etiquetas HTML5 como <header>, <main>, <nav>,
<footer>, <section>, y <article>.
3. Asegúrate de que todas las imágenes tengan textos alternativos descriptivos y
significativos.
4. Verifica y corrige la estructura de encabezados (<h1> a <h6>) para que sea
jerárquicamente correcta.
5. Implementa una navegación por teclado lógica y accesible.
6. Asegura un contraste de color adecuado entre el texto y el fondo (relación mínima de
4.5:1 para AA, 7:1 para AAA).
7. Añade etiquetas descriptivas a todos los campos de formulario.
8. Incluye instrucciones claras para los campos de formulario que requieran un formato
específico.
9. Asegúrate de que todos los elementos interactivos tengan un área de interacción
mínima de 44x44 píxeles.
10. Implementa un skip link al inicio de la página para saltar directamente al contenido
principal.
11. Asegúrate de que el idioma de la página esté correctamente especificado.
12. Proporciona subtítulos y transcripciones para contenido multimedia si es aplicable.
13. Evita el uso de atributos que dependan únicamente del color para transmitir información.
14. Asegúrate de que el contenido sea legible y funcional cuando se amplía hasta un 200%.
15. Verifica que todos los atributos aria-labelledby y aria-describedby referencien un id
existente en la página.
16. Asegura que los elementos referenciados por aria-labelledby y aria-describedby
contengan etiquetas o descripciones adecuadas.
17. Si la página no tiene un <h1>, agrégalo con un título claro y descriptivo.
18. Asegura que la jerarquía de encabezados sea coherente (<h1> → <h2> → <h3>, etc.).
19. Para <video> con audio, asegúrate de incluir subtítulos sincronizados (<track> con
kind="captions").
20. Para <audio> y <video>, proporciona una transcripción accesible en texto.
21. Verifica que el contenido multimedia tenga una alternativa textual adecuada para
usuarios con discapacidades auditivas.
Aplica estas modificaciones manteniendo la funcionalidad original del código. Comenta cada
cambio significativo para explicar su propósito en relación con la accesibilidad.

## Tools Used

-   AI Programming Assistants: ChatGPT, Perplexity
-   Accessibility Validation Tools:
    -   WAVE (Web Accessibility Evaluation Tool)
    -   Axe (Accessibility Testing Tool)
    -   Lighthouse (Google Chrome)

## Problems Found and Solutions

| Problem                               | Applied Solution                                                                                                                                            |
| :------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lack of semantic structure             | Implemented semantic HTML5 tags (`<header>`, `<main>`, `<nav>`, `<footer>`).                                                                                   |
| Images without alternative text        | Added descriptive `alt` attributes to all images.                                                                                                         |
| Forms without associated labels        | Added `<label>` elements and correctly associated them with form fields using the `for` attribute.                                                         |
| Insufficient color contrast           | Adjusted text and background colors to comply with required contrast ratios (minimum 4.5:1 for AA, 7:1 for AAA).                                            |
| Lack of hierarchical headings          | Restructured headings to follow a logical hierarchy from `<h1>` to `<h6>`.                                                                                 |
| Interactive elements without ARIA      | Added ARIA roles and attributes `aria-label` and `aria-describedby` to improve the accessibility of interactive elements.                                     |
| Inaccessible multimedia content        | Included subtitles for videos and transcripts for audios.                                                                                                  |
| ARIA attributes with broken references | Verified and corrected references in `aria-labelledby` and `aria-describedby` attributes to ensure they point to existing and descriptive elements.           |

## Validation Results

Below are the results of the validation tools before and after applying the prompt and making corrections.

### index1.html

-   Accessibility before: [Screenshot: Accessibility before index1]
-   Accessibility after: [Screenshot: Accessibility after index1\_accessible]

### index2.html

-   Accessibility before: [Screenshot: Accessibility before index2]
-   Accessibility after: [Screenshot: Accessibility after index2\_accessible]

### index3.html

-   Accessibility before: [Screenshot: Accessibility before index3]
-   Accessibility after: [Screenshot: Accessibility after index3\_accessible]

### index4.html

-   Accessibility before: [Screenshot: Accessibility before index4]
-   Accessibility after: [Screenshot: Accessibility after index4\_accessible]

## Conclusions

The developed prompt proved to be highly effective in improving the accessibility of HTML files, even in the most complex case of `index4.html`. The combination of the prompt, AI assistants, and validation tools allowed for the identification and resolution of a wide range of accessibility issues, complying with WCAG 2.2 A, AA, and AAA criteria.

# Generación de Código (HTML + CSS)
Quiero que generes **solo código**, sin explicaciones, usando **sintaxis Markdown** con bloques de código.

---

## INSTRUCCIONES GENERALES

Genera:

- Un archivo **HTML5 completo** con estructura semántica.
- Un archivo **CSS externo** llamado **styles.css**.
- SEO profesional en el `<head>`.
- Accesibilidad completa (roles, aria-label, alt, ARIA W3C).
- Schema.org en formato **JSON-LD**.
- Diseño responsivo básico.
- Código **minimalista**, sin frameworks ni JavaScript.

### ✔️ Reglas de CSS
- **CSS completamente DRY:** variables globales en `:root`, clases utilitarias, componentes modulares, sin repetición de reglas.
- Usa **selectores claros y específicos**, sin anidamientos innecesarios.
- Implementa **Flexbox** para layout (alineación, distribución y orden).
- Aplica metodología **BEM**: `bloque`, `bloque__elemento`, `bloque--modificador`.

### ✔️ Mobile‑First
- Estilos base para pantallas pequeñas.
- Diseño inicial simple y optimizado para móviles.
- Media queries con `min-width` para tablets y desktops.
- Construir primero la versión móvil y luego escalar.

### ✔️ Evita antipatrones CSS
- Nada de `!important`.
- Nada de selectores largos o demasiado específicos.
- Nada de anidamiento profundo.
- Nada de estilos inline.
- Nada de dependencias rígidas del DOM.
- Nada de modificadores BEM encadenados incorrectamente.

---

## ACCESIBILIDAD (POUR + WCAG 2.1 AA + ARIA + Formularios accesibles)

### ✔️ Principios POUR

**1. Perceptible**
- Todas las imágenes deben tener `alt` descriptivo.
- Contraste adecuado entre texto y fondo.
- Información visible y legible en cualquier dispositivo.

**2. Operable**
- Navegación completa por teclado.
- Controles accesibles y visibles.
- Sin elementos que parpadeen peligrosamente.

**3. Comprensible**
- Lenguaje claro y consistente.
- Formularios con etiquetas (`label`) correctamente asociadas.
- Mensajes de error claros y útiles.

**4. Robusto**
- HTML semántico.
- Compatible con lectores de pantalla.
- Sin hacks que rompan accesibilidad.

---

### ✔️ WCAG 2.1 Nivel AA

**1. Contraste y legibilidad**
- Contraste mínimo 4.5:1.
- Evitar fuentes pequeñas o ilegibles.

**2. Navegación por teclado**
- Toda la interfaz operable sin mouse.
- Foco visible en elementos interactivos.

**3. Tecnologías asistivas**
- Compatible con JAWS, NVDA, VoiceOver.
- Roles ARIA solo cuando HTML semántico no sea suficiente.
- Orden del DOM debe coincidir con el orden visual.

**4. Evitar contenido problemático**
- Sin animaciones que parpadeen más de 3 veces por segundo.
- Sin contenido que genere confusión cognitiva.

**5. Formularios accesibles**
- Cada campo con su `label` asociado mediante `for` + `id`.
- Mensajes de error anunciados con `aria-live="polite"`.
- Campos obligatorios indicados de forma accesible.
- Nada de placeholders como sustitutos de etiquetas.

**6. Estructura semántica**
- Encabezados en orden lógico (`h1`, `h2`, `h3`).
- Uso correcto de `main`, `nav`, `header`, `footer`, `section`, `article`.

---

### ✔️ ARIA W3C

- Roles ARIA solo cuando HTML semántico no sea suficiente.
- `aria-label` para elementos interactivos sin texto claro.
- `aria-labelledby` y `aria-describedby` para textos asociados.
- `aria-live="polite"` para mensajes dinámicos (errores).
- Roles ARIA deben coincidir con la función real del elemento.
- ARIA complementa, no reemplaza HTML semántico.
- Orden lógico del DOM para tecnologías asistivas.

---

## PALETA DE COLORES (minimalista y cálida)

- #2B2B2B (texto)
- #FAFAFA (fondo)
- #FF6F61 (acento cálido)
- #FFD54F (acento secundario)

---

## ESTRUCTURA DEL SITIO

1. **Barra de Navegación Principal**
   - role="navigation"
   - aria-label="navegación principal"
   - Enlaces: Inicio, Sobre mí, Trayectoria, Próximas presentaciones

2. **Hero Section**
   - Título principal
   - Subtítulo
   - Botón CTA

3. **Sobre Mí**
   - Imagen con alt descriptivo
   - Texto introductorio

4. **Trayectoria**
   - Grid con 3 eventos artísticos

5. **Próximas Presentaciones**
   - Grid con 2 eventos futuros

6. **Contáctame**
   - Nombre del artista
   - Email
   - Teléfono
   - Localización

7. **Pie de Página**
   - Derechos de autor

---

## HEAD COMPLETO (obligatorio)

Incluye:

- `<meta charset="UTF-8">`
- `<meta name="viewport">`
- `<title>`
- `<meta name="description">`
- `<meta name="keywords">`
- `<link rel="canonical">`
- Open Graph (`og:*`)
- Twitter Cards (`twitter:*`)
- Favicon
- Preload de styles.css
- Script JSON-LD con Schema.org (tipo Person + WebSite)

---

## RESTRICCIONES

- No incluyas explicaciones.
- No incluyas comentarios fuera del código.
- No uses JavaScript.
- No uses frameworks.
- No uses librerías externas.
- No inventes secciones adicionales.

---

## SALIDA

Genera ahora el **HTML + CSS** siguiendo todas las instrucciones anteriores.

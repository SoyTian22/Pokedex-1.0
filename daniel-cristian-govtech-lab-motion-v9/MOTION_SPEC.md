# Motion Design Spec - Daniel Cristian GovTech Lab

## Objetivo

Elevar la experiencia visual con un lenguaje premium, negro, neón y altamente interactivo para presentarle a Daniel una plataforma GovTech sofisticada.

## Patrones implementados

### 1. View Transitions

Uso conceptual de `document.startViewTransition` para que los cambios entre secciones no sean cortes bruscos sino transiciones suaves.

```css
::view-transition-old(root) {
  animation: vt-out .45s cubic-bezier(.4,0,.2,1);
}

::view-transition-new(root) {
  animation: vt-in .7s cubic-bezier(.16,1,.3,1);
}
```

### 2. Tarjetas con transición avanzada

```css
.card {
  transition-property: transform, opacity, background-color, border-color, box-shadow, filter;
  transition-duration: .55s;
  transition-timing-function: cubic-bezier(.16,1,.3,1);
  transition-delay: 0ms;
}
```

### 3. Navbar animada

La navegación usa cápsulas con hover, delay progresivo y activación visual clara. En mobile se convierte en una barra inferior tipo app.

### 4. Departamentos con relieve

Cada departamento se comporta como una tarjeta viva: al pasar el mouse sube, escala, satura e ilumina.

- Partido Nacional: celeste.
- Frente Amplio: negro.
- Partido Colorado: rojo.
- Otros: gris.

### 5. Smoke/Glow layer

Capa visual de profundidad con radial blur, mezcla tipo screen y movimiento lento.

### 6. Slider de soluciones

Tarjetas tipo slider con perspectiva, rotación y movimiento de profundidad.

## Siguientes mejoras posibles

- Integrar GSAP completo para timeline, draggable y advanced staggering.
- Añadir slider 3D con ScrollTrigger cuando el entorno permita dependencias externas.
- Convertir el mapa en SVG real con límites departamentales.
- Agregar dominio personalizado con Cloudflare/Vercel o un dominio propio.
- Separar repositorio exclusivo para producción.

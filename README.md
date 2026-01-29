# JocarsaCarrusel

Carrusel de imágenes ligero en **HTML + CSS + JavaScript puro**, sin dependencias externas.  
Convierte automáticamente un conjunto de `<img>` en un carrusel horizontal con botones de navegación.

🔹 Ideal para proyectos simples, landing pages, demos o sitios estáticos.  
🔹 Código claro, educativo y fácil de modificar.

---

## 📸 Demo rápida

```html
<div class="jocarsacarrusel">
  <img src="imagen1.jpg">
  <img src="imagen2.jpg">
  <img src="imagen3.jpg">
</div>

<link rel="stylesheet" href="https://jocarsa.github.io/jocarsacarrusel/jocarsacarrusel.css">
<script src="https://jocarsa.github.io/jocarsacarrusel/jocarsacarrusel.js"></script>
````

---

## 🇪🇸 Documentación en Español

### 📦 ¿Qué hace este carrusel?

* Toma todas las imágenes dentro del contenedor `.jocarsacarrusel`
* Las envuelve automáticamente en una `<section>`
* Desplaza el carrusel horizontalmente usando `left`
* Añade botones de navegación (◀ ▶)
* Usa `transition` CSS para animación suave

---

### 🧩 Estructura HTML requerida

```html
<div class="jocarsacarrusel">
  <img src="1.jpg">
  <img src="2.jpg">
  <img src="3.jpg">
</div>
```

⚠️ No es necesario añadir botones ni `<section>` manualmente.

---

### 🎨 CSS (estilos principales)

* Tamaño fijo por defecto: **1280×720**
* Bordes redondeados
* Sombra suave
* Overflow oculto para efecto carrusel

Puedes modificar fácilmente el tamaño cambiando:

```css
.jocarsacarrusel {
  width:1280px;
  height:720px;
}
```

Y en el JS:

```js
var anchura = 1280;
```

---

### ⚙️ Funcionamiento JavaScript

* Detecta todas las imágenes
* Las mueve dentro de un nuevo `<section>`
* Controla la posición con un contador
* Mueve el carrusel multiplicando `contador * anchura`

Ejemplo:

```js
nuevo_contenedor.style.left = contador * anchura + "px";
```

---

### ✅ Ventajas

* Sin librerías
* Muy ligero
* Ideal para aprender DOM
* Fácil de extender (autoplay, touch, responsive…)

---

## 🇬🇧 English Documentation

### 📦 What does this carousel do?

* Takes all `<img>` elements inside `.jocarsacarrusel`
* Wraps them automatically into a `<section>`
* Slides horizontally using CSS `left`
* Adds navigation buttons (◀ ▶)
* Uses CSS transitions for smooth animation

---

### 🧩 Required HTML structure

```html
<div class="jocarsacarrusel">
  <img src="1.jpg">
  <img src="2.jpg">
  <img src="3.jpg">
</div>
```

⚠️ No need to manually add buttons or `<section>`.

---

### 🎨 CSS overview

* Default size: **1280×720**
* Rounded corners
* Box shadow
* Hidden overflow for sliding effect

To change size, update:

```css
.jocarsacarrusel {
  width:1280px;
  height:720px;
}
```

And in JavaScript:

```js
var anchura = 1280;
```

---

### ⚙️ JavaScript logic

* Collects all images
* Moves them into a new `<section>`
* Controls position with a counter
* Updates `left` position on button click

Example:

```js
nuevo_contenedor.style.left = contador * anchura + "px";
```

---

### ✅ Advantages

* No dependencies
* Lightweight
* Educational DOM manipulation
* Easy to extend (autoplay, touch, responsive…)

---

## 📄 License

MIT License – free to use, modify and distribute.

---

## 👤 Author

**Jose Vicente Carratalá**
[https://github.com/jocarsa](https://github.com/jocarsa)

---

## 🚀 Ideas for future improvements

* Autoplay
* Responsive mode
* Touch / swipe support
* Infinite loop
* Indicators (dots)

---

Enjoy it and feel free to fork or improve it 🙂



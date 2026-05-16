# Verónica Arciniega — Portfolio

Portfolio profesional de diseñadora UX/UI, producto y gráfica.

## Estructura del repositorio

```
/
├── index.html          ← Página principal (no renombrar)
├── projects.json       ← Datos de proyectos (editar aquí para añadir proyectos)
├── assets/
│   ├── og-image.jpg    ← Imagen de preview para redes sociales (1200×630px)
│   ├── thunder-gym.jpg ← Imagen del proyecto 1
│   └── ...             ← Resto de imágenes de proyectos
├── Logo blanco.png     ← Logo para dark mode
├── Logo neg.png        ← Logo para light mode
└── FOTO4.jpg           ← Foto de perfil
```

## Cómo publicar en GitHub Pages

1. Crea un repositorio en GitHub con el nombre `averonicaarciniegap.github.io`
   (sustituye `averonicaarciniegap` por tu nombre de usuario exacto de GitHub)

2. Sube todos los archivos a la rama `main`

3. En el repositorio → Settings → Pages → Source: selecciona `main` → `/ (root)`

4. Tu portfolio estará disponible en: `https://averonicaarciniegap.github.io`

## Cómo añadir un proyecto nuevo

Abre `projects.json` y añade un objeto al array siguiendo esta estructura:

```json
{
  "id": "nombre-unico-del-proyecto",
  "category": "uxui",
  "color": "#6366f1",
  "titleEs": "Nombre en español",
  "titleEn": "Name in English",
  "tagEs": "Etiqueta en español",
  "tagEn": "Tag in English",
  "descEs": "Descripción en español.",
  "descEn": "Description in English.",
  "image": "assets/nombre-imagen.jpg",
  "tags": ["Figma", "UX Research"],
  "link": "https://figma.com/tu-prototipo"
}
```

**Categorías disponibles:**
- `uxui` → aparece en el filtro UX/UI
- `graphic` → aparece en el filtro Gráfico
- `product` → aparece en el filtro Producto

**El campo `link`** es opcional. Si lo dejas vacío (`""`), no aparece el botón "Ver proyecto".

## Imágenes

- Formato recomendado: **WebP** o JPG
- Tamaño recomendado para proyectos: **1280×720px** (ratio 16:9)
- Foto de perfil: **800×1000px** (ratio 4:5)
- Imagen Open Graph (`og-image.jpg`): **1200×630px**

## Actualizar la URL canónica

En `index.html`, busca estas líneas y actualiza tu URL real:

```html
<link rel="canonical" href="https://TU_USUARIO.github.io/">
<meta property="og:url" content="https://TU_USUARIO.github.io/">
```

## Tecnologías

- HTML5 semántico + CSS3 con variables custom
- JavaScript vanilla (sin frameworks)
- Google Fonts: Plus Jakarta Sans + Space Mono
- Sin dependencias de build (funciona directamente en GitHub Pages)

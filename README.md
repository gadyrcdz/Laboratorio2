# 🏍️ Super Motos Tech 2025 - Documentación CSS

Sitio web estático sobre el evento tecnológico de alto cilindraje, seguridad y rendimiento.

---

## 🌍 URL pública en Netlify
👉 [Sitio WEB](https://deploy-preview-1--incomparable-pika-f58c60.netlify.app/)

---

## 📋 Elementos CSS Aplicados en el Laboratorio

### 1. **Selectores de tipo**
- **`header`**: Estilos para el encabezado principal
- **`nav`**: Navegación principal del sitio
- **`section`**: Secciones de contenido (agenda, expositores, etc.)
- **`img`**: Imágenes del sitio con bordes y transiciones
- **`footer`**: Pie de página con fondo oscuro

### 2. **Selectores de clase**
- **`.btn`**: Botones de navegación y formulario
- **`.card`**: Tarjetas de expositores y contenido
- **`.badge`**: Etiquetas VIP en las tarjetas
- **`.cards-container`**: Contenedores de grid para organizar contenido
- **`.skip-link`**: Enlace de navegación rápida para accesibilidad

### 3. **Selectores de ID**
- **`#agenda`**: Sección principal de agenda del evento
- **`#expositores`**: Sección de expositores con grid layout
- **`#registro`**: Formulario de registro de participantes
- **`#ubicacion`**: Información de ubicación del evento
- **`#patrocinadores`**: Sección de logos de patrocinadores

### 4. **Selectores de atributo**
- **`a[target="_blank"]`**: Enlaces externos con icono y estilos especiales
- **`img[alt]`**: Imágenes con texto alternativo y efectos hover
- **`input[type="email"]`**: Campo de email con gradiente de fondo
- **`button[type="submit"]`**: Botón de envío del formulario

### 5. **Combinadores**
- **`nav a + a`**: Espaciado entre enlaces adyacentes en la navegación
- **`.card p`**: Párrafos dentro de las tarjetas con estilos específicos
- **`header > nav`**: Navegación directa dentro del header
- **`.tag ~ .tag`**: Etiquetas hermanas con espaciado
- **`tbody tr:nth-child(2n)`**: Filas alternas en tablas

### 6. **Pseudo-clases de estado**
- **`:hover`**: Efectos al pasar el mouse en botones, enlaces e imágenes
- **`:focus-visible`**: Contorno de enfoque para accesibilidad
- **`:active`**: Estados activos de botones
- **`:visited`**: Enlaces visitados
- **`:focus`**: Estados de enfoque en formularios

### 7. **Pseudo-clases estructurales**
- **`:first-child`**: Primer elemento de listas con peso bold
- **`:last-child`**: Último elemento de listas con estilo italic
- **`:nth-child(2n)`**: Elementos pares con fondo alternado
- **`:nth-child(2n+1)`**: Elementos impares

### 8. **Especificidad (!important e inline style)**
- **`.card .badge`**: Uso de `!important` para sobrescribir estilos base
- **`h2` con `style="margin-bottom:24px;"`**: Estilo inline en título de expositores

### 9. **Box model**
- **`.card`**: Padding, margin y border para crear tarjetas
- **`section`**: Márgenes y padding para espaciado entre secciones
- **`nav a`**: Padding y border para botones de navegación
- **`form`**: Padding y margin para formularios

### 10. **Overflow**
- **`.card p`**: Control de overflow en párrafos de tarjetas con `max-height: 4.2em`, `overflow: hidden` y `text-overflow: ellipsis` - Ejemplo en la tarjeta de Lin Jarvis con texto largo

### 11. **Flexbox**
- **`nav ul`**: Navegación principal con `display: flex` para alinear enlaces
- **`#patrocinadores .cards-container`**: Contenedor de logos con flexbox para centrado

### 12. **Grid**
- **`#expositores .cards-container`**: Grid layout para organizar tarjetas de expositores
- **`#patrocinadores .cards-container`**: Grid para logos de patrocinadores

### 13. **Position relative/absolute**
- **`.badge`**: Posicionamiento absoluto en las tarjetas para etiquetas VIP
- **`header`**: Posición relativa para el header principal

### 14. **Responsive Design (Mobile-First)**
- **Media Queries**: Breakpoints en 768px (tablet) y 1024px (desktop)
- **Menú hamburguesa**: `.menu-toggle` con `aria-controls` y `aria-expanded` para móvil
- **Grid responsive**: Cards con 1 columna (móvil), 2 columnas (tablet), 3 columnas (desktop)
- **Navegación adaptativa**: Oculto en móvil, visible en tablet/desktop
- **Tipografía escalable**: Tamaños de fuente que se adaptan al dispositivo
- **Imágenes responsive**: `max-width: 100%` y `height: auto` para evitar desbordamiento

---


## 📁 Estructura de Archivos

```
├── index.html
├── styles/
│   ├── base.css      (Variables CSS y estilos base)
│   ├── layout.css    (Layout y estructura)
│   ├── components.css (Componentes reutilizables)
│   └── overrides.css (Sobrescrituras y ajustes)
├── assets/
│   └── (Imágenes del proyecto)
└── README.md
```

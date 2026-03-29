# 🔥 Fuego Lento & Co.

Un recetario interactivo minimalista de cocina argentina tradicional, inspirado en las enseñanzas de Doña Petrona C. de Gandulfo y los clásicos de nuestra gastronomía.

![Fuego Lento & Co.](https://img.shields.io/badge/Fuego%20Lento%20%26%20Co.-Cocina%20Argentina-amber)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

## ✨ Características

### 🎙️ Narrador AI Amigable
- **Síntesis de voz en español** con tono cálido y pausado
- **Tres perfiles de voz**: Amigable, Tranquila y Alegre
- **Selección inteligente** de voces femeninas naturales (Paulina, Mónica, Sabina)
- **Velocidad adaptada** para cocinar sin prisa (0.8x - 0.95x)
- **Guía paso a paso** con prefijos motivadores ("Perfecto, ahora...", "Muy bien...")

### 📸 Imágenes Reales
- **9 recetas clásicas** con fotografías auténticas:
  - Empanadas de Carne
  - Locro Criollo
  - Humitas en Chala
  - Matambre Arrollado
  - Tarta de Ricota
  - Pastel de Papas
  - Medialunas de Manteca
  - Milanesas a la Napolitana
  - Chocotorta
- **Subida de fotos** al agregar nuevas recetas (drag & drop)
- **Vista previa instantánea** con validación de tamaño (max 5MB)

### 🎨 Diseño Minimalista
- **Paleta de colores**: Tonos stone (piedra) y ámbar cálido
- **Tipografía**: Playfair Display (títulos) + Inter (cuerpo)
- **Textura sutil**: Overlay de grano para sensación artesanal
- **Animaciones suaves**: Hover effects y transiciones fluidas
- **Totalmente responsive**: Adaptable a móvil, tablet y desktop

### 🍳 Funcionalidades Culinarias
- **Filtros por categoría**: Con Carne, Vegetarianas, Dulces, Clásicos
- **Checklist de ingredientes**: Tachar items al usarlos
- **Progreso visual**: Barra de avance en la preparación
- **Consejos de Doña Petrona**: Tips específicos en cada receta
- **Agregar recetas propias**: Formulario completo con categorización

## 🚀 Uso

1. **Abrir** el archivo `index.html` en cualquier navegador moderno
2. **Navegar** por las recetas usando los filtros de categoría
3. **Seleccionar** una receta para ver detalles completos
4. **Activar el narrador** para guía paso a paso con voz
5. **Agregar recetas** propias con el botón "+" en el header

### Atajos de Teclado
| Tecla | Acción |
|-------|--------|
| `→` o `Espacio` | Siguiente paso |
| `←` | Paso anterior |
| `Esc` | Cerrar receta |

## 🛠️ Tecnologías

- **HTML5** - Estructura semántica
- **CSS3** - Tailwind CSS + estilos personalizados
- **JavaScript** - Lógica interactiva y Web Speech API
- **Web Speech API** - Síntesis de voz nativa del navegador
- **FileReader API** - Carga de imágenes locales

## 📱 Compatibilidad

- Chrome/Edge (recomendado para mejor soporte de voces)
- Firefox
- Safari (limitaciones en voces en español)
- Opera

> **Nota**: La síntesis de voz funciona mejor en Chrome y Edge debido a su amplia biblioteca de voces en español.

## 📝 Estructura de Datos

Las recetas siguen el formato:

```javascript
{
  id: number,
  title: string,
  category: 'carne' | 'vegetariano' | 'dulce' | 'clasico',
  time: number, // minutos
  difficulty: 'Baja' | 'Media' | 'Alta',
  image: string, // URL o Base64
  description: string,
  ingredients: string[],
  steps: string[],
  tips: string // Consejo de Doña Petrona
}

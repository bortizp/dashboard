# TechTrends Dashboard - Instrucciones

## 📋 Descripción del Proyecto

Este es un dashboard interactivo para TechTrends, una tienda en línea de gadgets tecnológicos. El dashboard permite visualizar y analizar datos de ventas de forma clara y profesional.

## 🚀 Cómo Usar el Dashboard

### Abrir el Dashboard:
1. Abre el archivo `index.html` en tu navegador web favorito (Chrome, Firefox, Edge, Safari)
2. El dashboard cargará automáticamente los datos del archivo CSV
3. Verás 4 tarjetas de métricas principales y 4 gráficos interactivos

### Funcionalidades:

#### Métricas Principales (Tarjetas Superiores):
- **Ventas Totales**: Suma de todas las ventas en dólares
- **Total Transacciones**: Número total de ventas realizadas
- **Producto Más Vendido**: El producto con mayores ingresos
- **País con Más Ventas**: El país que genera más ingresos

#### Gráficos Disponibles:
1. **📈 Ventas Totales Mensuales**: Gráfico de línea que muestra la evolución de ventas mes a mes
2. **🏆 Top 5 Productos Más Vendidos**: Gráfico de barras con los 5 productos que generan más ingresos
3. **💳 Métodos de Pago**: Gráfico circular mostrando la distribución de métodos de pago (Tarjeta, PayPal, Transferencia)
4. **🌎 Ventas por País**: Gráfico de dona mostrando la distribución de ventas por país

#### Filtros Interactivos:
- **Filtrar por Producto**: Selecciona un producto específico para ver solo sus datos
- **Filtrar por Mes**: Filtra datos de un mes específico
- **Filtrar por País**: Muestra datos de un país en particular

**Nota**: Los filtros se actualizan en tiempo real. Al cambiar un filtro, todas las métricas y gráficos se actualizan automáticamente.

## 🛠️ Tecnologías Utilizadas

### Frontend:
- **HTML5**: Estructura del dashboard
- **CSS3**: Estilos y diseño visual
  - Diseño responsivo (se adapta a móvil y escritorio)
  - Gradientes modernos
  - Animaciones y transiciones suaves
- **JavaScript Vanilla**: Lógica de negocio y procesamiento de datos
  - Lectura y parseo del archivo CSV
  - Cálculo de métricas agregadas
  - Gestión de filtros interactivos

### Librería de Gráficos:
- **Chart.js v4.4.0**: Librería profesional para crear gráficos interactivos
  - Gráficos de línea (line charts)
  - Gráficos de barras (bar charts)
  - Gráficos circulares (pie charts)
  - Gráficos de dona (doughnut charts)

## 📊 Preguntas de Negocio Respondidas

El dashboard responde las siguientes preguntas clave del equipo de TechTrends:

### 1. ¿Cuáles son los productos más vendidos?
- **Respuesta**: El gráfico "Top 5 Productos Más Vendidos" muestra los productos ordenados por ingresos totales
- **Resultado**: Teclado Mecánico es el producto más vendido con $2,550 en ventas totales

### 2. ¿Cómo varían las ventas a lo largo del tiempo?
- **Respuesta**: El gráfico "Ventas Totales Mensuales" muestra la tendencia de ventas mes a mes
- **Observación**: Se pueden identificar meses con mayores ventas (junio y septiembre con ~$1,100) y meses más bajos (noviembre con ~$400)

### 3. ¿Qué métodos de pago son más utilizados?
- **Respuesta**: El gráfico "Métodos de Pago" muestra la distribución
- **Resultado**: La Tarjeta de crédito es el método más usado (52%), seguido de PayPal (28%) y Transferencia (20%)

### 4. ¿Cómo se distribuyen las ventas por región/país?
- **Respuesta**: El gráfico "Ventas por País" muestra la distribución geográfica
- **Resultado**: Colombia lidera con 27% de las ventas, seguido por México (23%), Argentina (19%), Chile (17%) y Perú (14%)

## 📁 Estructura de Archivos

```
dashboard/
├── index.html                      # Dashboard principal (archivo único HTML+CSS+JS)
├── chart.js                        # Librería Chart.js para gráficos
├── datos taller de software-1.csv  # Datos de ventas (100 transacciones)
├── package.json                    # Configuración npm (opcional)
├── .gitignore                      # Archivos a ignorar en git
├── README.md                       # Documentación original
└── INSTRUCCIONES.md               # Este archivo
```

## 🎯 Características del Diseño

- **Moderno y Profesional**: Colores atractivos con gradiente púrpura
- **Fácil de Entender**: Iconos y etiquetas claras
- **Interactivo**: Filtros que actualizan todo en tiempo real
- **Responsivo**: Funciona en computadoras, tablets y móviles
- **Animaciones Suaves**: Efectos hover y transiciones elegantes

## 💡 Cómo Funciona Internamente

### 1. Carga de Datos:
```javascript
// El dashboard usa fetch() para leer el archivo CSV
// Luego parsea cada línea y crea objetos JavaScript
```

### 2. Procesamiento:
```javascript
// Calcula métricas agregadas:
// - Suma de ventas totales
// - Conteo de transacciones
// - Agrupación por producto, mes, país, método de pago
```

### 3. Visualización:
```javascript
// Usa Chart.js para crear gráficos dinámicos
// Cada gráfico se actualiza cuando cambias los filtros
```

### 4. Interactividad:
```javascript
// Los filtros tienen event listeners
// Cuando cambias un filtro, se recalculan las métricas
// y se actualizan todos los gráficos automáticamente
```

## 🎥 Puntos Clave para la Presentación en Video

1. **Introducción (30 seg)**:
   - "Este es el dashboard de TechTrends, una solución simple para visualizar ventas"
   - Mostrar la pantalla completa del dashboard

2. **Métricas Principales (30 seg)**:
   - Explicar las 4 tarjetas superiores
   - "Podemos ver ventas totales de $9,208.50 en 100 transacciones"

3. **Gráficos (1 min)**:
   - Explicar cada gráfico brevemente
   - Destacar insights: "Junio y septiembre fueron los mejores meses"

4. **Filtros Interactivos (1 min)**:
   - Demostrar filtrado por producto (ej: Smartwatch)
   - Mostrar cómo se actualizan las métricas y gráficos
   - "Al filtrar por Smartwatch, vemos 12 transacciones por $2,040"

5. **Tecnologías (30 seg)**:
   - "Desarrollado con HTML, CSS y JavaScript"
   - "Uso Chart.js para los gráficos profesionales"
   - "Todo funciona sin servidor, solo abriendo el archivo HTML"

6. **Código (1.5 min)**:
   - Abrir index.html en editor
   - Mostrar estructura HTML (header, métricas, filtros, gráficos)
   - Mostrar CSS (estilos, gradientes, responsive)
   - Mostrar JavaScript (loadData, updateCharts, filters)

7. **Cierre (30 seg)**:
   - "Dashboard simple, funcional y fácil de entender"
   - "Responde todas las preguntas del negocio"
   - "Listo para usar y presentar"

## ✅ Cumplimiento de Requisitos

- ✅ **Extracción de Datos**: CSV cargado y parseado correctamente
- ✅ **Transformación de Datos**: Métricas agregadas calculadas (suma, conteo, agrupación)
- ✅ **Visualización**: 4 gráficos profesionales con Chart.js
- ✅ **Dashboard**: Interfaz limpia y profesional en una sola página
- ✅ **Interactividad**: 3 filtros funcionales que actualizan todo en tiempo real
- ✅ **Diseño Atractivo**: Colores modernos, gradientes, animaciones
- ✅ **Código Limpio**: Bien estructurado y comentado
- ✅ **Simplicidad**: Implementación básica pero completa

## 📝 Notas Adicionales

- El dashboard es **completamente estático** - no requiere servidor ni base de datos
- Los datos se cargan directamente del CSV usando JavaScript
- Es **fácil de extender** - puedes agregar más gráficos o filtros
- El código está **bien comentado** para facilitar la comprensión
- Es **responsive** - se ve bien en cualquier dispositivo

---

**Desarrollado por**: Bastián Alexander Ortiz Pizarro
**Curso**: Ingeniería en Software
**Profesor**: Victor Heughes Escobar Jeria
**Institución**: TechTrends E-commerce Dashboard Project

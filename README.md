# BR Registry · Dashboard

Dashboard web para la gestión y monitoreo de **registros**, con visualización de métricas y datos en tiempo real.

## 📋 ¿Qué es?

Sistema administrativo que permite consultar, filtrar y visualizar registros almacenados en **Supabase** (base de datos PostgreSQL en la nube). Diseñado para uso interno o restringido.

## 🖥️ Servicios del Dashboard

| Servicio | Descripción |
|----------|-------------|
| **Visualización de Datos** | Tabla principal con registros de la tabla `BR_REGISTRY` |
| **Gráficos Estadísticos** | Gráficos interactivos (Chart.js) con métricas clave |
| **Filtro por Fechas** | Calendario con selección de rango para filtrar datos |
| **Panel de Métricas** | KPIs y resumen de datos en tiempo real |

## 🛠️ Configuración

1. Copia `config.example.js` y renómbralo a `config.js`
2. Ingresa tus credenciales de Supabase:
   ```javascript
   const URL_BASE = 'https://tu-proyecto.supabase.co';
   const KEY      = 'tu-key-public';
   const TABLE    = 'BR_REGISTRY';
   ```

## 📦 Stack Tecnológico
- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Base de Datos**: Supabase (PostgreSQL)
- **Gráficos**: Chart.js
- **Efectos 3D**: Three.js (intro animada)

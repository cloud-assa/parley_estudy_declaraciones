# BR Menores · Dashboard

Panel administrativo interactivo para la gestión y visualización de datos (probablemente declaraciones o registros menores), integrado con **Supabase** para el almacenamiento y **Chart.js** para analíticas.

## 🚀 Funcionalidades Principales
- **Dashboard en Tiempo Real**: Visualización de métricas clave mediante gráficos interactivos.
- **Gestión de Datos**: Interfaz optimizada para el manejo de registros en la tabla `BR_MENORES`.
- **Filtros Avanzados**: Selector de fechas tipo calendario con rangos personalizados.
- **Interfaz Moderna**: UI oscura (dark mode) con animaciones fluidas y diseño responsivo.

## 🛠️ Configuración (Importante)
El proyecto utiliza un archivo `config.js` para conectar con la base de datos, el cual **no se incluye en el repositorio** por seguridad.

1. Localiza el archivo `config.example.js` en la raíz.
2. Crea una copia y cámbiale el nombre a `config.js`.
3. Rellena los campos con tus credenciales de Supabase:
   ```javascript
   const URL_BASE = 'TU_URL_DE_SUPABASE';
   const KEY      = 'TU_KEY_DE_ANON_PUBLIC';
   const TABLE    = 'BR_MENORES';
   ```

## 📦 Tecnologías
- **Frontend**: HTML5, CSS3 (Variables modernas, Flexbox/Grid), JavaScript (Vanilla).
- **Librerías**: Three.js (Intro/Efectos), Chart.js (Gráficos), Inter & Fira Code (Fuentes).
- **Backend**: Supabase (BaaS).

---
*Este proyecto está configurado para un despliegue rápido. Asegúrate de tener Git configurado correctamente para futuras actualizaciones.*

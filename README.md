# BR Registry · Dashboard

Panel administrativo para visualización y monitoreo de datos con métricas e indicadores en tiempo real.

## 📊 ¿Qué muestra?

Dashboard interactivo que presenta:

- **Panel Principal**: Vista general con KPIs y métricas resumidas
- **Gráficos Interactivos**: Visualización de datos mediante Chart.js
- **Tabla de Registros**: Exploración detallada de cada entrada
- **Filtro por Fechas**: Selector de rango para consultar períodos específicos
- **Análisis de Datos**: Perfil retórico, tópicos por partido y más

## ⚙️ Configuración

1. Edita `config.js` en la carpeta `docs/`
2. Verifica que los datos coincidan con tu proyecto en Supabase:
   ```javascript
   const URL_BASE = 'https://tu-proyecto.supabase.co';
   const KEY      = 'tu-key-public';
   const TABLE    = 'NOMBRE_DE_TU_TABLA';
   ```

## 🔧 Requisitos de la Base de Datos

La tabla en Supabase debe tener los siguientes campos:
- `FECHA_PUBLICACION` (fecha)
- `TITULO` (texto)
- `AUTOR` (texto)
- `PARTIDO` (texto)
- `SENTIMIENTO` (texto)
- `PALABRAS_CLAVE` (texto)
- Otros campos según análisis

Además, en Supabase:
1. Ve a **Authentication** → **Settings** → desactiva **Enable confirm email**
2. Ve a tu tabla → **Replication** → asegura tener al menos 1 replica
3. Ve a **SQL Editor** y ejecuta para permitir acceso anónimo:

```sql
ALTER TABLE "NOMBRE_DE_TU_TABLA" ENABLE ROW LEVEL SECURITY;
CREATE POLICY "Allow anonymous reads" ON "NOMBRE_DE_TU_TABLA" FOR SELECT USING (true);
```

## 🛠️ Requisitos

- Navegador web moderno
- Acceso a internet

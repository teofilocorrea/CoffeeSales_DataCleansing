# 🧱 Registro de Entorno Local DuckDB

**Versión del documento:** 1.0  
**Fecha de creación:** 2025-11-11  
**Autor:** Teófilo Correa Rojas  
**Propósito:** Registrar la configuración técnica del entorno local DuckDB utilizado para exploración, validación y análisis de datasets (EDA Preliminar y EDA Analítico).

---

## 📁 1. Información General del Entorno

| Parámetro | Detalle                  |
|------------|--------------------------|
| **Nombre del entorno** | Local DuckDB – Sandbox   |
| **Tipo de motor** | DuckDB (embebido)        |
| **Archivo principal** | `--`                     |
| **Tamaño inicial** | 12 KB                    |
| **Fecha de creación** | 2025-11-10               |
| **Herramienta de conexión** | DataGrip 2025.2.4          |
| **Versión de DuckDB** | 1.3.1                    |
| **Modo de conexión** | Local file (no servidor) |
| **Acceso verificado** | ✅ Conexión exitosa       |

---

## 🗃️ 2. Estructura de Schemas

| Schema | Descripción | Estado   |
|---------|--------------|----------|
| `raw` | Zona de aterrizaje (datasets fuente sin transformación) | ✅ Creado |
| `staging` | Área de limpieza y tipificación de datos | ❌ No     |
| `analytics` | Modelos y vistas listos para análisis | ❌ No    |

**Script ejecutado:**
```sql
CREATE SCHEMA IF NOT EXISTS raw;
CREATE SCHEMA IF NOT EXISTS staging;
CREATE SCHEMA IF NOT EXISTS analytics;
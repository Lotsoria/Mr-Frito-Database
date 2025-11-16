# Mr-Frito-Database – Visión general

Carpeta con los artefactos de base de datos MySQL usados por el proyecto Mr. Frito. Incluye modelo, scripts y seeds iniciales.

## Contenido
- `schema.mwb` / `schema.mwb.bak`: modelo MySQL Workbench.
- `schema_v1.pdf`: diagrama exportado del modelo.
- `script.sql`: DDL generado (creación de tablas, índices, llaves foráneas).
- `inserts.sql`: datos semilla básicos.

La estructura coincide con el esquema Prisma consumido por el backend (`api-mrfrito/prisma/schema.prisma`), con tablas como `usuarios`, `canales`, `ventas`, `gastos`, `categorias_gasto`, `presupuestos`, `alertas`, etc.

## Uso sugerido
- Crear base de datos MySQL y ejecutar `script.sql`, luego `inserts.sql` para datos iniciales.
- Verificar/ajustar nombres de la base de datos y credenciales según tu entorno antes de importar.
- Si trabajas con Prisma en el backend, mantén sincronizados este modelo y `prisma/schema.prisma` para evitar divergencias.

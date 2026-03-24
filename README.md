# Depto Gastos

App para dividir gastos entre Feli, Bau y Helen.

## Deploy en 3 pasos

### Paso 1 — Google Apps Script (backend)

1. Abrí el Google Sheet donde querés guardar los datos
2. Menú → **Extensiones → Apps Script**
3. Borrá el código que aparece y pegá todo el contenido de `Code.gs`
4. Guardá (Ctrl+S) y poné un nombre (ej: "Depto Gastos API")
5. Click en **Implementar → Nueva implementación**
   - Tipo: **Aplicación web**
   - Ejecutar como: **Yo**
   - Quién tiene acceso: **Cualquier usuario**
6. Click **Implementar** → copiá la URL que aparece (empieza con `https://script.google.com/macros/s/...`)

> ⚠️ Cada vez que modifiques el script, tenés que crear una **nueva implementación** para que los cambios tomen efecto.

### Paso 2 — GitHub Pages (frontend)

1. Creá un repo nuevo en github.com (ej: `depto-gastos`)
2. Subí `index.html` al repo
3. Ir a **Settings → Pages → Source: Deploy from branch → main / (root)**
4. En unos segundos la app queda en `https://TU-USUARIO.github.io/depto-gastos`

### Paso 3 — Conectar

1. Abrí la app en el navegador
2. Pegá la URL del Apps Script en el banner amarillo
3. Click **Guardar**

Listo. Las tres pueden abrir la misma URL y los datos se sincronizan via Google Sheet.

## Estructura de datos

La Sheet "Gastos" tiene estas columnas:

| id | fecha | descripcion | categoria | tipo | pagador | total | parte_feli | parte_bau | parte_helen | notas |

## Compartir con Feli y Helen

Mandales la URL de GitHub Pages. No necesitan cuenta ni login.

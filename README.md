# Gestión Económica-Financiera — Campo Cuatro

App de una sola página (`index.html`) con evolución de ingresos y egresos, comparación por concepto y por cuenta contable, comparación de períodos/años, e índices. Los datos y el logo están embebidos en el propio archivo — no necesita servidor, base de datos, ni instalar nada.

## Publicar en GitHub Pages (primera vez)

**1. Creá una cuenta en GitHub** (si no tenés una todavía): [github.com/signup](https://github.com/signup).

**2. Creá un repositorio nuevo:**
   - Arriba a la derecha, click en el **+** → **New repository**.
   - Ponele un nombre, por ejemplo `campo-cuatro-financiero`.
   - Dejalo en **Public** (con cuenta gratis, Pages solo funciona en repos públicos).
   - No tildes "Add a README" — dejalo vacío. Click **Create repository**.

**3. Subí el archivo:**
   - En la página del repo recién creado, click en **uploading an existing file** (o "Add file → Upload files" si ya tiene contenido).
   - Arrastrá el `index.html` que te pasé.
   - Abajo, click **Commit changes**.

**4. Activá GitHub Pages:**
   - En el repo, andá a la pestaña **Settings**.
   - En el menú de la izquierda, click en **Pages**.
   - En "Build and deployment → Source" elegí **Deploy from a branch**.
   - En "Branch" elegí **main** y carpeta **/ (root)**. Click **Save**.

**5. Esperá 1-2 minutos** y refrescá la página de Settings → Pages. Va a aparecer un cartel verde con el link, algo como:
   `https://tu-usuario.github.io/campo-cuatro-financiero/`

   Ese es el link que podés guardar como favorito o compartir con quien necesite ver el tablero.

## Actualizar los datos

Cuando tengas números nuevos (por ejemplo, egresos de julio en adelante):

1. Subime acá en el chat el archivo Excel actualizado.
2. Te devuelvo un `index.html` nuevo con los datos incorporados.
3. En GitHub, entrá al repositorio → click en `index.html` → ícono de lápiz (**Edit**) o directamente "Add file → Upload files" arrastrando el nuevo archivo con el mismo nombre → **Commit changes**.
4. GitHub Pages se actualiza solo, en 1-2 minutos.

No hace falta tocar nada más — el diseño, el logo, los gráficos y los filtros de período son siempre los mismos; solo cambia el bloque de datos.

## Actualizar los datos

Cuando tengas números nuevos (por ejemplo, egresos de julio en adelante):

1. Subime acá en el chat el archivo Excel actualizado.
2. Te devuelvo un `index.html` nuevo con los datos incorporados.
3. Reemplazá el archivo en el repositorio (subiendo el nuevo `index.html` sobre el viejo, mismo nombre). GitHub Pages se actualiza solo en 1-2 minutos.

No hace falta tocar nada más — el diseño, los gráficos y los filtros de período son siempre los mismos; solo cambia el bloque de datos.

## Qué incluye

- **Selector de período**: elegís qué meses/años entran en todos los cálculos (arriba de todo, con atajos "Todo" / "Últimos 12 meses" / "Ninguno").
- **Evolución**: ingresos, egresos y resultado mes a mes.
- **Por Concepto**: ranking de ingresos (Unidad de Negocio) y egresos (Grupo de Gastos), con detalle por cuenta contable al hacer click en cada concepto.
- **Índices**: margen mensual/acumulado, ratio ingresos/egresos, estructura de egresos, cobertura de egresos con el ingreso de Leche, y variación interanual por mes. Se comparan períodos con el mismo selector de arriba.
- **Toggle $ / U$D** en el encabezado.

## Criterio de neto

Igual que en el Excel: se excluye el IVA (débito fiscal en ventas / crédito fiscal en compras, ya discriminado en el Concepto "IVA" del archivo fuente) y las Inversiones (Grupo de Gastos "BIENES DE CAPITAL" — compra de bienes de uso), que no inciden en el resultado del período. Las Mejoras (mantenimiento) sí quedan incluidas, por ser gasto operativo. Todo lo demás (préstamos, socios) queda incluido tal cual figura en origen.

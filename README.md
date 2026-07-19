# 🚗 FlotaPrecioJusto — Control de Vehículos

Sistema profesional de gestión de flota para **Precio Justo**. Administra vehículos, conductores, mantenimientos y gastos con interfaz moderna y funcionalidades avanzadas.

---

## ✨ Características Principales

### 📊 Dashboard
- **Estadísticas en vivo**: Total de vehículos, activos, conductores y alertas
- **Cards de vehículos**: Vista rápida de los principales con estado y conductor asignado
- **Sistema de alertas**: Documentos vencidos (SOAT, técnicomecanica, licencias, seguros)

### 🚙 Gestión de Vehículos
- ✏️ **Editar/Crear** vehículos con todos los detalles
- 🗑️ **Eliminar** vehículos
- 📋 Seguimiento de documentos: SOAT, Técnicomecanica, Seguro, Tarjeta Operacional
- 🔍 **Búsqueda instantánea** por placa, nombre o marca
- Estados: Activo, Mantenimiento, Inactivo

### 👤 Gestión de Conductores
- ✏️ **Editar/Crear** conductores
- 🗑️ **Eliminar** conductores
- 📱 Teléfono, cédula, licencia con fechas de vencimiento
- ⚠️ Alertas de documentos vencidos
- Asignación de vehículos

### 🔧 Mantenimientos
- 📝 Registro completo: tipo, taller, repuestos, mano de obra
- 🗒️ Descripción y historial
- 📅 Programación del próximo mantenimiento (fecha y km)
- ✏️ **Editar/eliminar** registros
- 🔍 Búsqueda por vehículo

### 💰 Gastos Varios
- Categorías: Combustible, Peaje, Estacionamiento, Lavada, Multas, Reparación, Otros
- 💵 Valor con formato de moneda
- 📝 Descripción del gasto
- ✏️ **Editar/eliminar** gastos
- 🔍 Búsqueda rápida

### 📋 Reportes Mensuales
- 📊 Análisis mensual por vehículo
- 💹 Desglose de mantenimientos vs otros gastos
- 🖨️ **Botón Imprimir** — Genera PDF profesional listo para imprimir
- 📥 **Exportar a CSV** — Vehículos, conductores, mantenimientos, gastos
- 📤 **Exportar a JSON** — Base completa o solo vehículos

---

## 🎮 Guía de Uso

### Botón 💾 Backup (en la esquina superior derecha)

#### Descargar Backup
1. Haz clic en **💾 Backup** en la barra superior
2. Selecciona **"Descargar Backup Completo"**
3. Se descargará un archivo JSON con todos tus datos: `backup_flota_YYYY-MM-DD.json`
4. Guárdalo en un lugar seguro (nube, USB, etc.)

#### Restaurar desde Backup
1. Haz clic en **💾 Backup**
2. En "Restaurar desde Backup", selecciona el archivo JSON descargado
3. Haz clic en **"Restaurar"**
4. ⚠️ **ADVERTENCIA**: Esto sobrescribirá TODOS los datos actuales
5. La app se recargará automáticamente

### Botón 🖨️ Imprimir (solo en Reportes)

1. Abre la pestaña **"📋 Reportes"**
2. Selecciona el mes que deseas imprimir
3. Haz clic en **"🖨️ Imprimir"**
4. Se abrirá una ventana con el reporte formateado profesionalmente
5. Usa **Ctrl+P** (o Cmd+P en Mac) para imprimir o guardar como PDF
6. El PDF incluye:
   - Detalles por vehículo
   - Tabla de mantenimientos
   - Tabla de otros gastos
   - Gasto total de la flota

### Botón 📊 Exportar (en Reportes)

#### Exportar como CSV
1. Ve a **"📋 Reportes"**
2. Haz clic en **"📊 Exportar"**
3. Selecciona qué deseas exportar:
   - **Vehículos** → `vehiculos_precioJusto.csv`
   - **Conductores** → `conductores_precioJusto.csv`
   - **Mantenimientos** → `mantenimientos_precioJusto.csv`
   - **Gastos** → `gastos_precioJusto.csv`
   - **Reporte Completo** → Unión de mantenimientos + gastos
4. Los archivos se descargan y puedes abrirlos en Excel

#### Exportar como JSON
1. Ve a **"📋 Reportes"**
2. Haz clic en **"📊 Exportar"**
3. Selecciona:
   - **Base Completa** → Todos los datos en un JSON
   - **Solo Vehículos** → Solo los vehículos en JSON

### Botones de Edición ✏️

En cada tabla (Conductores, Mantenimientos, Gastos):
- **✏️ Editar** — Abre el modal con los datos actuales para modificar
- **🗑️ Eliminar** — Borra el registro (con confirmación)

En la tarjeta de vehículos:
- Haz clic en la tarjeta o en el botón **"Editar"** para abrir el modal
- Modifica los datos
- Haz clic en **"Guardar"**

---

## 🔐 Seguridad de Datos

### Almacenamiento
- **localStorage**: Todos los datos se guardan automáticamente en el navegador
- **Cambios automáticos**: Cada operación (crear, editar, eliminar) se guarda de inmediato

### Backup Manual
- Descarga backups regularmente usando el botón 💾 **Backup**
- Guarda en múltiples lugares (nube, USB)
- Recomendado: Descarga un backup cada semana

### Eliminación Segura
En **Backup** → **Opciones Avanzadas**:
- **Limpiar Base de Datos**: Elimina TODOS los datos (requiere confirmación doble)

---

## 📱 Compatibilidad

- ✅ **Navegadores Modernos**: Chrome, Firefox, Safari, Edge
- ✅ **Dispositivos**: Desktop, Tablet, Móvil (PWA)
- ✅ **Offline**: Funciona sin conexión a internet (datos en localStorage)
- ✅ **Instalable**: Instálalo como app en tu dispositivo

---

## 🌍 Formatos Soportados

### CSV (Excel)
- Separador: `;` (punto y coma)
- Codificación: UTF-8 con BOM
- Compatible con: Excel, Google Sheets, LibreOffice

### JSON
- Formato completo de la base de datos
- Válido para restauración
- Fácil de compartir

### PDF (Imprimir)
- Profesional y listo para presentar
- Incluye resumen ejecutivo
- Tabla detallada por vehículo

---

## 💡 Tips & Trucos

1. **Búsqueda rápida**: Usa Ctrl+F en cualquier tabla para filtrar
2. **Exportar periódico**: Descarga backups cada semana
3. **Documentos próximos a vencer**: El dashboard te muestra alertas
4. **Reportes profesionales**: El PDF es listo para cliente o presentación
5. **Múltiples navegadores**: Cada navegador tiene su propia copia de datos

---

## ⚙️ Opciones Avanzadas

### En el modal Backup:

**Última Modificación**
- Muestra cuándo fue el último cambio en la base de datos

**Limpiar Base de Datos**
- ⚠️ **PELIGROSO**: Elimina todo
- Requiere escribe "BORRAR" dos veces
- No tiene vuelta atrás (a menos que tengas un backup)

---

## 📞 Soporte

**Desarrollada por**: Vibras Positivas HM
**Derechos de Autor Reservados** © 2026

---

## 🎯 Casos de Uso

### Caso 1: Backup Semanal
1. Lunes por la mañana → Descarga backup
2. Guarda en Google Drive o Dropbox
3. Usa durante la semana
4. Repite cada lunes

### Caso 2: Reportar a Gerencia
1. Ve a Reportes
2. Selecciona el mes
3. Haz clic en "🖨️ Imprimir"
4. Guarda como PDF
5. Envía por email

### Caso 3: Migrar a Otra Computadora
1. Descarga backup en computadora actual
2. Instala FlotaPrecioJusto en nueva computadora
3. Abre FlotaPrecioJusto
4. Restaura desde el backup
5. ¡Listo! Todos tus datos están sincronizados

### Caso 4: Compartir Datos con Equipo
1. Exporta a JSON o CSV
2. Comparte el archivo
3. El equipo puede abrirlo en Excel o JSON viewer

---

## ✅ Checklist de Implementación

- [x] Gestión de vehículos (CRUD completo)
- [x] Gestión de conductores (CRUD completo)
- [x] Mantenimientos (registrar, editar, eliminar)
- [x] Gastos (registrar, editar, eliminar)
- [x] Reportes mensuales detallados
- [x] Sistema de alertas
- [x] Botón Backup y Restaurar
- [x] Botón Imprimir
- [x] Exportar CSV
- [x] Exportar JSON
- [x] Interfaz responsive
- [x] PWA ready
- [x] Datos persistentes (localStorage)

---

**¡Disfruta de FlotaPrecioJusto!** 🚗✨

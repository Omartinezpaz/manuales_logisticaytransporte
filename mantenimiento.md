# Manual de Gestión de Mantenimiento (SILT-PEQUIVEN)

Este manual detalla el control de Órdenes de Trabajo (OT) y el mantenimiento preventivo y correctivo de la flota.

## 1. Órdenes de Trabajo (OT)
Toda intervención mecánica debe estar respaldada por una OT con número único (ej. OT-00001).

### Tipos de Mantenimiento:
1.  **Preventivo**: Basado en el kilometraje recorrido. El sistema alerta al acercarse al umbral de servicio.
2.  **Correctivo**: Debido a fallas imprevistas o incidentes. Se gestiona con prioridad URGENTE.

## 2. Roles y Autorizaciones
- **Coordinadores**: Únicos autorizados para **Crear** y **Rechazar** OTs.
- **Supervisores**: Encargados de **Verificar** la correcta ejecución técnica.
- **Analistas Administrativos**: Únicos que pueden **Finalizar** la OT una vez cargados los costos reales.

## 3. Repuestos e Insumos
- Cada OT permite registrar el **Stock de Repuestos** utilizados (Spare Parts).
- El sistema valida la disponibilidad en almacén antes de permitir el registro.
- Se debe indicar el costo por unidad y la cantidad.

## 4. Proveedores y Talleres
- Las OTs se asignan a **Proveedores (Suppliers)** internos o externos.
- El proveedor puede visualizar sus OTs asignadas a través de su portal específico.

## 5. Control de Costos (CECO)
- La OT requiere un **Centro de Costos (CECO)** asociado.
- Antes de la creación, el sistema verifica que el CECO tenga **presupuesto mensual disponible**.
- El presupuesto se reduce automáticamente al finalizar la OT con el costo real.

# Manual de Gestión de Combustible (SILT-PEQUIVEN)

Este manual detalla el control de abastecimiento de combustible y el seguimiento de consumo y eficiencia.

## 1. Registro de Abastecimiento
Toda carga de combustible debe ser registrada en tiempo real por el **Conductor** a través de la aplicación móvil.

### Datos Obligatorios:
- **Estación de Servicio**: Nombre de la estación.
- **Tipo de Combustible**: Diesel/Gasolina (debe coincidir con el tipo del vehículo).
- **Litros** y **Costo por Litro**: El sistema calcula el costo total.
- **Kilometraje (Odómetro)**: Al momento de la carga.

## 2. Validaciones de Negocio
Para evitar errores de carga o fraudes, el sistema implementa:
- **Validación de Secuencia**: El nuevo kilometraje debe ser mayor al anterior y no tener un aumento mayor a 5.000 km en un solo registro.
- **Detección de Anomalías**: El sistema compara el rendimiento (km/L) con el promedio histórico (últimos 30 días). Si la eficiencia cae más del **25%** respecto al promedio, se genera una alerta automática.

## 3. Gastos y Facturas
- Cada registro de combustible puede estar asociado a una **Factura (Invoice)** digitalizada.
- Se recomienda subir la foto del ticket o comprobante de carga directamente desde el dispositivo móvil.

## 4. Control Presupuestario
- El costo del combustible se deduce automáticamente del **Balance de Presupuesto (BudgetBalance)** mensual del Centro de Costo (CECO) asignado al vehículo.
- Si el CECO no tiene fondos suficientes, el sistema registrará el consumo con una advertencia administrativa.

## 5. Reportes de Eficiencia
El sistema ofrece tableros para analizar:
- Consumo promedio por unidad de flota.
- Histórico de costos por estación de servicio.
- Alertas recurrentes de anomalías por conductor o vehículo.

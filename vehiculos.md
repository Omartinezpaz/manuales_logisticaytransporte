# Manual de Gestión de Vehículos (SILT-PEQUIVEN)

Este manual describe el funcionamiento y las reglas de negocio del módulo de flota vehicular.

## 1. Introducción
El módulo de vehículos permite el control exhaustivo de la flota de PEQUIVEN, asegurando que cada unidad cumpla con los requisitos técnicos y legales.

## 2. Registro de un Nuevo Vehículo
Solo **Administradores** o **Coordinadores** pueden registrar vehículos.
- **Placa**: Debe seguir el formato venezolano (ABC123, AB1C23D o AA000AA).
- **VIN (Chasis)**: Código de 17 caracteres alfanuméricos.
- **Marca, Modelo y Año**: Datos obligatorios de identificación.

## 3. Estados del Vehículo
1. **Activo**: Disponible.
2. **Mantenimiento**: En taller, no disponible para traslados.
3. **Inactivo**: Fuera de servicio temporal o definitivo.

## 4. Gestión de Kilometraje y Seguros
- El kilometraje no puede ser menor al registro anterior.
- El sistema valida la vigencia del seguro (SOAT/Póliza).

## 5. Actualización de Datos (Seguridad)
- **Admin/Coord**: Edición directa.
- **Conductor**: Genera una **Solicitud de Servicio (SOL-VEH-...)** que requiere aprobación.

## 6. Bajas (Soft Delete)
No se puede eliminar un vehículo con **traslados en progreso**.

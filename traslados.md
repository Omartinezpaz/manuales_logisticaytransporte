# Manual de Control de Traslados (SILT-PEQUIVEN)

Este manual describe el ciclo de vida de una operación de transporte, desde la solicitud hasta el cierre operativo.

## 1. El Ciclo de Vida del Traslado
Cada traslado pasa por diferentes estados controlados por el sistema:
1.  **Pendiente**: Nueva solicitud creada.
2.  **Confirmado / Asignado**: Vehículo y conductor vinculados.
3.  **En Progreso**: El conductor inició el viaje.
4.  **Completado**: Finalización exitosa.
5.  **Cancelado**: Suspensión del servicio.

## 2. Flujo de Aprobaciones (Workflow)
Para garantizar el control presupuestario, el sistema requiere validaciones jerárquicas:
- **Coordinador**: Revisa la factibilidad técnica y asigna recursos.
- **Gerente**: Aprueba el gasto asociado al centro de costos.
- **Supervisor**: Verifica el cumplimiento de seguridad industrial antes del inicio.

## 3. Notificaciones por Telegram
El sistema envía alertas automáticas en cada etapa clave:
- Al **Conductor** cuando se le asigna un nuevo viaje.
- Al **Solicitante** cuando su traslado cambia de estado.
- Al **Staff Gerencial** sobre nuevas solicitudes críticas.

## 4. Datos del Operativo
- **Ruta**: Origen y Destino obligatorio.
- **Carga**: Tipo de material y peso estimado en toneladas.
- **Kilometraje**: Se registra el odómetro inicial y final para el cálculo de rendimiento.
- **Duración**: Estimada vs Real para análisis de eficiencia logística.

## 5. Cierre Operativo
Para completar un traslado, el conductor debe reportar cualquier novedad y el supervisor debe validar el cierre en el sistema.

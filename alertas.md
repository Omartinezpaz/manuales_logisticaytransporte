# Manual de Usuario: Gestión de Alertas

El módulo de **Alertas** es el centro de monitoreo proactivo del sistema SILT-PEQUIVEN. Su función es notificar a los usuarios sobre eventos críticos, desviaciones presupuestarias y necesidades operativas inmediatas.

## 1. Tipos de Alertas y Severidad

El sistema clasifica las alertas según su naturaleza y el impacto en la operación:

| Tipo | Descripción | Severidad Típica |
| :--- | :--- | :--- |
| **Límite de Presupuesto** | El consumo de un Centro de Costo alcanzó un umbral (90% o 100%). | CRITICAL / WARNING |
| **Anomalía de Combustible** | Desviación mayor al 75% en el consumo promedio histórico. | WARNING |
| **Stock Bajo** | Material con inventario igual o inferior al stock mínimo definido. | WARNING |
| **Mantenimiento Preventivo** | Vehículo próximo a alcanzar el kilometraje de servicio. | INFO / WARNING |
| **Vencimiento de Documentos** | Documentos (Licencias, Seguros) próximos a expirar (30 días). | WARNING |
| **Nueva Solicitud** | Ingreso de una solicitud de servicio que requiere atención. | INFO |

## 2. Gestión de Alertas

### 2.1 Visualización y Filtrado
Desde el panel de alertas, el usuario puede filtrar por:
- **Estado**: Leídas, No leídas, Resueltas, Pendientes.
- **Severidad**: Crítica (Rojo), Advertencia (Amarillo), Informativa (Azul).
- **Entidad**: Vehículo, Conductor, Centro de Costo, Proveedor.

### 2.2 Marcar como Leída
Al visualizar una alerta, esta cambia automáticamente su estado a "leída". Los usuarios pueden usar la opción **"Marcar todas como leídas"** para limpiar el panel global de notificaciones.

### 2.3 Resolución de Alertas
Las alertas críticas (como anomalías o límites de presupuesto) requieren una **resolución explícita**:
1. Seleccionar la alerta.
2. Ingresar una **nota de resolución** (justificación técnica o administrativa).
3. Cambiar el estado a **Resuelto**.
*Nota: El sistema registra quién resolvió la alerta y en qué fecha para fines de auditoría.*

## 3. Notificaciones Externas
Dependiendo del perfil del usuario, las alertas también se envían a través de canales secundarios:
- **Telegram**: Notificaciones inmediatas para Gerentes, Supervisores y Coordinadores sobre incidentes y presupuestos.
- **Dashboard**: Resumen de indicadores (KPIs) con el conteo de alertas críticas pendientes.

## 4. Reglas de Acceso (RBAC)
- **Administradores/Gerentes**: Ven todas las alertas del sistema y sedes.
- **Mecánicos/Proveedores**: Solo visualizan alertas de **mantenimiento** y **stock bajo** de materiales vinculados.
- **Conductores**: Solo visualizan alertas relacionadas con sus **vehículos asignados** y sus **documentos personales**.

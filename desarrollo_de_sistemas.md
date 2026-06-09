```mermaid
flowchart TD
    A([Inicio]) --> B[Usuario presenta solicitud formal de<br/>desarrollo o modificación de sistema<br/>al Coordinador TI]

    B --> C{¿Solicitud es viable<br/>técnica y presupuestariamente?}

    C -- No --> D[Notificar al usuario con<br/>justificación técnica del rechazo]
    D --> FIN1([Fin])

    C -- Sí --> E[Levantar requerimientos funcionales y<br/>no funcionales mediante entrevistas,<br/>talleres y revisión documental<br/>con usuarios clave]

    E --> F[Elaborar ERS y someter a revisión<br/>y firma de aprobación del<br/>usuario solicitante]

    F --> G[Diseñar arquitectura del sistema,<br/>modelo de datos y prototipos<br/>de interfaz. Presentar al Coordinador TI]

    G --> H[Desarrollar el sistema según<br/>especificaciones aprobadas aplicando<br/>estándares de codificación segura]

    H --> I[Ejecutar pruebas unitarias, de integración<br/>y de seguridad. Corregir los<br/>defectos encontrados]

    I --> J{¿Sistema aprueba<br/>pruebas de aceptación<br/>del usuario - UAT?}

    J -- No --> H

    J -- Sí --> K[Coordinador TI aprueba y ejecuta el<br/>despliegue en el ambiente de producción]

    K --> L[Realizar seguimiento post-implementación<br/>durante 30 días. Atender incidencias<br/>de estabilización]

    L --> FIN2([Fin])
```

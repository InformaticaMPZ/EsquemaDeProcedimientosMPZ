```mermaid
flowchart TD
    A([Inicio]) --> B[Recibir petición de servicio<br/>Llamada, correo, chat o HelpDesk]

    B --> C[Analizar si puede resolverse de forma remota]

    C --> D{¿Se resolvió de forma remota?}

    D -- Sí --> FIN1([Fin])

    D -- No --> E[Registrar tarea en Microsoft Planner<br/>y asignar prioridad]

    E --> F[Coordinador analiza prioridad]

    F --> G{¿Es urgente?}

    G -- No --> H[Caso en cola de espera]
    H --> F

    G -- Sí --> I[Asignar técnico y notificar al usuario]

    I --> J[Técnico se moviliza y ejecuta la solución]

    J --> K[Completar bitácora en Planner<br/>y obtener firma de conformidad]

    K --> FIN2([Fin])
```
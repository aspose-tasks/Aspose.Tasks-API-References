---
title: TaskLink.LinkLagTimeSpan
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TaskLink propiedad. Obtiene o establece la duración del retraso según LagFormat.
type: docs
weight: 50
url: /es/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Obtiene o establece la duración del retraso, según LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Al intentar establecer el valor para TaskLinks donde LagFormat es TimeUnitType.Percent. |

### Observaciones

El retraso del enlace puede ser un valor porcentual (LagFormat es TimeUnitType.Percent). En este caso, la duración se calcula como un porcentaje de la duración de PredTask. De lo contrario, el método devuelve el valor TimeSpan que representa el retraso de TaskLink.

### Ver también

* class [TaskLink](../)
* espacio de nombres [Aspose.Tasks](../../tasklink/)
* asamblea [Aspose.Tasks](../../../)



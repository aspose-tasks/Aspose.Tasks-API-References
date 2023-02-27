---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TimephasedDataCollection método. Selecciona todas las fases de tiempo entrestartTime yfinishTime . Tiene complejidad Olog n en caso promedio.
type: docs
weight: 120
url: /es/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Selecciona todas las fases de tiempo entre*startTime* y*finishTime* . Tiene complejidad O(log n) en caso promedio.

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Tipo de fases de tiempo a seleccionar. |
| startTime | DateTime | Inicio del intervalo. |
| finishTime | DateTime | Fin del intervalo. |

### Valor_devuelto

Devuelve una nueva instancia de lista de[`TimephasedDataCollection`](../) datos ordenados por propiedad de inicio.

### Ver también

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* espacio de nombres [Aspose.Tasks](../../timephaseddatacollection/)
* asamblea [Aspose.Tasks](../../../)



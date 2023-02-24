---
title: TimephasedData.CreateCostTimephased
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TimephasedData método. Crea e inicializa una nueva instancia delTimephasedData clase para datos de fase temporal basados en costos.
type: docs
weight: 20
url: /es/net/aspose.tasks/timephaseddata/createcosttimephased/
---
## TimephasedData.CreateCostTimephased method

Crea e inicializa una nueva instancia del[`TimephasedData`](../) clase para datos de fase temporal basados en costos.

```csharp
public static TimephasedData CreateCostTimephased(int uid, DateTime start, DateTime finish, 
    double value, TimeUnitType timeUnit, TimephasedDataType type)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| uid | Int32 | UID de la tarea. |
| start | DateTime | fecha-hora de inicio. |
| finish | DateTime | Finalizar fecha-hora. |
| value | Double | Valor de coste. |
| timeUnit | TimeUnitType | Tipo de unidad de tiempo. |
| type | TimephasedDataType | Tipo de datos de fase temporal. |

### Valor_devuelto

Una instancia de la[`TimephasedData`](../) class para datos de fase temporal basados en costes.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Si se especificó un valor de costo negativo. |

### Ver también

* enum [TimeUnitType](../../timeunittype/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* espacio de nombres [Aspose.Tasks](../../timephaseddata/)
* asamblea [Aspose.Tasks](../../../)



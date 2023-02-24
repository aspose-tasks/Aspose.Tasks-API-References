---
title: TimephasedData.CreateUnitTimephased
second_title: Referencia de Aspose.Tasks para la API de .NET
description: TimephasedData método. Crea e inicializa una nueva instancia delTimephasedData clase para datos de fase temporal basados en unidades de una asignación de un recurso material.
type: docs
weight: 30
url: /es/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Crea e inicializa una nueva instancia del[`TimephasedData`](../) clase para datos de fase temporal basados en unidades de una asignación de un recurso material.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| uid | Int32 | UID de la tarea. |
| start | DateTime | Fecha-hora de inicio. |
| finish | DateTime | Finalizar fecha-hora. |
| units | Double | Número de unidades. |
| type | TimephasedDataType | Tipo de datos de fase temporal. |

### Valor_devuelto

Una instancia de la[`TimephasedData`](../) class para datos de fase temporal basados en costes.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentException | Si se especificó una cantidad negativa de unidades. |

### Ver también

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* espacio de nombres [Aspose.Tasks](../../timephaseddata/)
* asamblea [Aspose.Tasks](../../../)



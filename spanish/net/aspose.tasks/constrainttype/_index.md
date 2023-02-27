---
title: Enum ConstraintType
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.ConstraintType enumeración. Especifica la restricción en la fecha de inicio o finalización de una tarea.
type: docs
weight: 330
url: /es/net/aspose.tasks/constrainttype/
---
## ConstraintType enumeration

Especifica la restricción en la fecha de inicio o finalización de una tarea.

```csharp
public enum ConstraintType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | El valor no se definió en el archivo de proyecto original. |
| AsSoonAsPossible | `0` | [`Start`](../tsk/start/) y[`Finish`](../tsk/finish/) fechas de[`Task`](../task/) están programados ASAP con respecto al padre[`Start`](../tsk/start/) y[`Finish`](../tsk/finish/)fechas y considerando[`TaskLinks`](../project/tasklinks/) . |
| AsLateAsPossible | `1` | [`Start`](../tsk/start/) y[`Finish`](../tsk/finish/) fechas de[`Task`](../task/) están programados ALAP con respecto al padre[`Start`](../tsk/start/) y[`Finish`](../tsk/finish/)fechas y considerando[`TaskLinks`](../project/tasklinks/) . |
| MustStartOn | `2` | Debe comenzar el |
| MustFinishOn | `3` | Debe terminar el |
| StartNoEarlierThan | `4` | Empezar no antes de |
| StartNoLaterThan | `5` | Empezar a más tardar el |
| FinishNoEarlierThan | `6` | Terminar no antes de |
| FinishNoLaterThan | `7` | Finalizar antes de |

### Observaciones

Al exportar a XML, los valores no definidos se eliminarán del XML resultante.

### Ver también

* espacio de nombres [Aspose.Tasks](../../aspose.tasks/)
* asamblea [Aspose.Tasks](../../)



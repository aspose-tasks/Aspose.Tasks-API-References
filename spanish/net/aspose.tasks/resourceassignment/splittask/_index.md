---
title: ResourceAssignment.SplitTask
second_title: Referencia de Aspose.Tasks para la API de .NET
description: ResourceAssignment método. Divide la tarea en dos partes.
type: docs
weight: 750
url: /es/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

Divide la tarea en dos partes.

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| start | DateTime | El comienzo de la interrupción del trabajo para dividir en función de. |
| finish | DateTime | El final de la interrupción del trabajo para dividir en función de. |
| calendar | Calendar | El calendario en el que se dividirá según. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentOutOfRangeException | Se lanza cuando la fecha de inicio es anterior a la fecha de inicio de la asignación. |
| ArgumentOutOfRangeException | Se lanza cuando la fecha de finalización es posterior a la fecha de finalización de la tarea. |

### Ver también

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* espacio de nombres [Aspose.Tasks](../../resourceassignment/)
* asamblea [Aspose.Tasks](../../../)



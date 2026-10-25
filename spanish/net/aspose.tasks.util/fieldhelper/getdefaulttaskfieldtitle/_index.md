---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método FieldHelper. Devuelve un título predeterminado del campo de tarea específico"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

Devuelve un título predeterminado del campo de tarea específico.

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskKey | TaskKey | Campo de tarea para obtener un título predeterminado. |

### Valor devuelto

Un título predeterminado del campo de tarea específico si el campo puede mostrarse en la vista de MS Project, null en caso contrario.

## Ejemplos

Muestra cómo obtener el título predeterminado del campo para el campo de tarea específico.

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### Ver también

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)



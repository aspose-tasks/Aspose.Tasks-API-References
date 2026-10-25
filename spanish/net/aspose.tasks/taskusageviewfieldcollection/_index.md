---
title: "Clase TaskUsageViewFieldCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TaskUsageViewFieldCollection. Representa una colección de valores de TaskUsageViewField."
type: docs
weight: 2500
url: /es/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

Representa una colección de valores de [`TaskUsageViewField`](../taskusageviewfield/).

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | Devuelve una lista que contiene todos los elementos de esta colección. |

## Ejemplos

Muestra cómo trabajar con la colección de campos de una instancia de TaskUsageView.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Se puede transformar la colección en una lista de TaskUsageViewField.
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Ver también

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



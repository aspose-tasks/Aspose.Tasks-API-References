---
title: "TaskUsageView.FieldCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TaskUsageView. Obtiene el objeto TaskUsageViewFieldCollection de este TaskUsageView"
type: docs
weight: 10
url: /es/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Obtiene el objeto [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) de este TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Ejemplos

Muestra cómo leer los campos de vista de uso de tareas.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Ver también

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)



---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskUsageViewFieldCollection. Devuelve una lista que contiene todos los elementos de esta colección"
type: docs
weight: 20
url: /es/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

Devuelve una lista que contiene todos los elementos de esta colección.

```csharp
public IList<TaskUsageViewField> ToList()
```

### Valor devuelto

devuelve una lista que contiene todos los elementos de esta colección.

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)



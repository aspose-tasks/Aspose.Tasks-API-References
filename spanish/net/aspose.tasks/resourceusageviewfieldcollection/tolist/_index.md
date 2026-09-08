---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceUsageViewFieldCollection. Convierte la instancia de la clase ResourceUsageViewFieldCollection en una lista que contiene las instancias de la clase ResourceUsageViewField"
type: docs
weight: 20
url: /es/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

Convierte la instancia de la clase [`ResourceUsageViewFieldCollection`](../) en una lista que contiene las instancias de la clase [`ResourceUsageViewField`](../../resourceusageviewfield/).

```csharp
public IList<ResourceUsageViewField> ToList()
```

### Valor devuelto

La instancia de la clase [`ResourceUsageViewFieldCollection`](../) convertida en una lista que contiene las instancias de la clase [`ResourceUsageViewField`](../../resourceusageviewfield/).

## Ejemplos

Muestra cómo trabajar con la colección de campos de una instancia ResourceUsageView.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// Se puede transformar la colección en una lista de ResourceUsageViewField
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### Ver también

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)



---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceUsageViewFieldCollection. Devuelve un enumerador para esta colección"
type: docs
weight: 10
url: /es/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

Devuelve un enumerador para esta colección.

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### Valor devuelto

un enumerador para esta colección.

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



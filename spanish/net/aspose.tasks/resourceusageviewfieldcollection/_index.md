---
title: "Clase ResourceUsageViewFieldCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.ResourceUsageViewFieldCollection. Representa una colección de valores ResourceUsageViewField"
type: docs
weight: 1830
url: /es/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

Representa una colección de valores [`ResourceUsageViewField`](../resourceusageviewfield/).

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | Devuelve un enumerador para esta colección. |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | Convierte la instancia de la clase `ResourceUsageViewFieldCollection` en una lista que contiene las instancias de la clase [`ResourceUsageViewField`](../resourceusageviewfield/). |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



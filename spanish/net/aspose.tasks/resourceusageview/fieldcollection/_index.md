---
title: "ResourceUsageView.FieldCollection"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ResourceUsageView. Obtiene el objeto ResourceUsageViewFieldCollection de este ResourceUsageView."
type: docs
weight: 10
url: /es/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Obtiene el objeto [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) de este ResourceUsageView.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Ejemplos

Muestra cómo leer los campos de vista de uso de recursos.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Ver también

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)



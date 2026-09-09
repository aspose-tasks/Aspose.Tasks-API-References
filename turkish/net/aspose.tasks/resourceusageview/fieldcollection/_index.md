---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceUsageView özelliği. Bu ResourceUsageView'in ResourceUsageViewFieldCollection nesnesini alır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Bu ResourceUsageView'in [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) nesnesini alır.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Örnekler

Kaynak kullanım görünüm alanlarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Ayrıca Bakınız

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)



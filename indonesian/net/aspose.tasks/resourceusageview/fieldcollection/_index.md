---
title: "ResourceUsageView.FieldCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ResourceUsageView. Mendapatkan objek ResourceUsageViewFieldCollection dari ResourceUsageView ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

Mendapatkan objek [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) dari ResourceUsageView ini.

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## Contoh

Menampilkan cara membaca bidang tampilan penggunaan sumber daya.

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Lihat Juga

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)



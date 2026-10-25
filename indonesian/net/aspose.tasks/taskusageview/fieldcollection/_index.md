---
title: "TaskUsageView.FieldCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TaskUsageView. Mendapatkan objek TaskUsageViewFieldCollection dari TaskUsageView ini"
type: docs
weight: 10
url: /id/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Mendapatkan objek [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) dari TaskUsageView ini.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Contoh

Menunjukkan cara membaca bidang tampilan penggunaan tugas.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Lihat Juga

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)



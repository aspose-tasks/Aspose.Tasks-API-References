---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskUsageView özelliği. Bu TaskUsageView'in TaskUsageViewFieldCollection nesnesini alır"
type: docs
weight: 10
url: /tr/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Bu TaskUsageView'in [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) nesnesini alır.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Örnekler

Görev kullanım görünümü alanlarını nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Ayrıca Bakınız

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)



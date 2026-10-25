---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskUsageView eigenschap. Haalt het TaskUsageViewFieldCollection-object van deze TaskUsageView op"
type: docs
weight: 10
url: /nl/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Haalt het [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) object van deze TaskUsageView op.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Voorbeelden

Toont hoe taakgebruikweergavevelden te lezen.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### Zie ook

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)



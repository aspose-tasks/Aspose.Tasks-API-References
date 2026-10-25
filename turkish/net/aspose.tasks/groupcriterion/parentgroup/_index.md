---
title: "GroupCriterion.ParentGroup"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GroupCriterion özelliği. GroupCriterion nesnesinin üst öğesini alır."
type: docs
weight: 100
url: /tr/net/aspose.tasks/groupcriterion/parentgroup/
---
## GroupCriterion.ParentGroup property

[`GroupCriterion`](../) nesnesinin üst öğesini alır.

```csharp
public Group ParentGroup { get; }
```

## Örnekler

Bir grup kriteriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Index: " + criterion.Index);
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Kriterin arka plan desenini okuyun.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

if (group == criterion.ParentGroup)
{
    Console.WriteLine("Parent Group is equal to task Group.");
}

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Ayrıca Bakınız

* class [Group](../../group/)
* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)



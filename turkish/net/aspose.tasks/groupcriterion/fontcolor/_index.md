---
title: "GroupCriterion.FontColor"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "GroupCriterion özelliği. Bir grup tanımında kriter olarak kullanılan bir alan için yazı tipinin rengini alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks/groupcriterion/fontcolor/
---
## GroupCriterion.FontColor property

Bir grup tanımında kriter olarak kullanılan bir alanın yazı tipi rengini alır veya ayarlar.

```csharp
public Color FontColor { get; set; }
```

## Örnekler

Bir grup kriterinin özelliklerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// Kriterin arka plan desenini okuyun.
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### Ayrıca Bakınız

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)



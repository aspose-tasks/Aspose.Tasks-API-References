---
title: "GroupCriterion.Ascending"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GroupCriterion. Получает или задает значение, указывающее, сортируется ли поле, используемое в качестве критерия в определении группы, по возрастанию. Ложно, если поле сортируется по убыванию."
type: docs
weight: 20
url: /ru/net/aspose.tasks/groupcriterion/ascending/
---
## GroupCriterion.Ascending property

Получает или задает значение, указывающее, сортируется ли поле, используемое в качестве критерия в определении группы, по возрастанию. False, если поле сортируется по убыванию.

```csharp
public bool Ascending { get; set; }
```

## Примеры

Показывает, как читать свойства группового критерия.

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

// читать фоновый шаблон критерия  
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### См. также

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)



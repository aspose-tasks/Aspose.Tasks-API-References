---
title: "TaskUsageView.FieldCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TaskUsageView. Получает объект TaskUsageViewFieldCollection этого TaskUsageView"
type: docs
weight: 10
url: /ru/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

Получает объект [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) этого TaskUsageView.

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## Примеры

Показывает, как читать поля представления использования задач.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### См. также

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)



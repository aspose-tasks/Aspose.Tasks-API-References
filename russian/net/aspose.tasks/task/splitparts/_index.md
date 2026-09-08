---
title: "Task.SplitParts"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает коллекцию SplitPart, представляющую части задачи"
type: docs
weight: 1110
url: /ru/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Получает коллекцию SplitPart, представляющую части задачи.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Примеры

Показывает, как отобразить разделённые части задачи.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Доступ к задаче 
var task = project.RootTask.Children.GetById(4);

// Отобразить разделённые части задачи
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### См. также

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



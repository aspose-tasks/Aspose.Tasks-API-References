---
title: "Task.Successors"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает объект TaskCollection, содержащий всех последователей этого объекта Task"
type: docs
weight: 1200
url: /ru/net/aspose.tasks/task/successors/
---
## Task.Successors property

Получает объект [`TaskCollection`](../../taskcollection/), содержащий всех последователей этого объекта Task.

```csharp
public TaskCollection Successors { get; }
```

### Возвращаемое значение

Экземпляр только для чтения класса [`TaskCollection`](../../taskcollection/).

## Примеры

Показывает, как прочитать последователей задачи.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### См. также

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



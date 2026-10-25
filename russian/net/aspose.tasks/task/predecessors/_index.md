---
title: "Task.Predecessors"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает объект TaskCollection, который содержит всех предшественников этого объекта Task"
type: docs
weight: 980
url: /ru/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Получает объект [`TaskCollection`](../../taskcollection/), который содержит всех предшественников этого объекта Task.

```csharp
public TaskCollection Predecessors { get; }
```

### Возвращаемое значение

Экземпляр только для чтения класса [`TaskCollection`](../../taskcollection/).

## Примеры

Показывает, как прочитать предшественников задачи.

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### См. также

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



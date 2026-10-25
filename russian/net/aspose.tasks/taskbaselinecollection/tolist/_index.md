---
title: "TaskBaselineCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskBaselineCollection. Преобразует объект TaskBaselineCollection в список объектов TaskBaseline"
type: docs
weight: 60
url: /ru/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

Преобразует объект TaskBaselineCollection в список объектов [`TaskBaseline`](../../taskbaseline/).

```csharp
public List<TaskBaseline> ToList()
```

### Возвращаемое значение

Список объектов [`TaskBaseline`](../../taskbaseline/).

## Примеры

Показывает, как работать с коллекциями базовых линий задач.

```csharp
var project = new Project();

// создать базовые линии проекта
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// печать базовых линий задач
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// давайте очистим все базовые линии
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### См. также

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)



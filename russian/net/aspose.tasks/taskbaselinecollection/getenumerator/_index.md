---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskBaselineCollection. Возвращает перечислитель для этой коллекции"
type: docs
weight: 40
url: /ru/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

Возвращает перечислитель для этой коллекции.

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### Возвращаемое значение

перечислитель для этой коллекции.

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



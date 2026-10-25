---
title: "Task.Baselines"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Получает или задает коллекцию значений baseline задачи"
type: docs
weight: 130
url: /ru/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Получает или задает коллекцию базовых значений задачи.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Примеры

Показывает, как прочитать baseline задачи.

```csharp
var project = new Project();

// установить baseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Отображение продолжительности базового плана задачи
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### См. также

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



---
title: "TaskBaseline.GetHashCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskBaseline. Возвращает значение хеш‑кода для экземпляра класса TaskBaseline."
type: docs
weight: 110
url: /ru/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

Возвращает значение хеш‑кода для экземпляра класса [`TaskBaseline`](../).

```csharp
public override int GetHashCode()
```

### Возвращаемое значение

возвращает значение хеш‑кода для этого объекта.

## Примеры

Показывает, как получить хеш‑код базового плана задачи.

```csharp
var project = new Project();

// создание TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// отображение длительности базовой линии задачи
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// хеш‑код календаря равен номеру базового плана
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### См. также

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)



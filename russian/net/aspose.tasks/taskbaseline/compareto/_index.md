---
title: "TaskBaseline.CompareTo"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskBaseline. Реализация интерфейса IComparable. Сравнивает данный экземпляр с указанным объектом Baseline"
type: docs
weight: 90
url: /ru/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

Реализация интерфейса IComparable. Сравнивает этот экземпляр с указанным объектом Baseline.

```csharp
public int CompareTo(TaskBaseline other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | TaskBaseline | указанный объект Baseline, с которым сравнивается этот экземпляр. |

### Возвращаемое значение

возвращает -1, если этот экземпляр меньше указанного объекта, 1, если этот экземпляр больше указанного объекта; в противном случае возвращает 0.

## Примеры

Показывает, как проверить равенство базовых линий.

```csharp
var project = new Project();

// создание TaskBaseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// отображение длительности базовой линии задачи
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// равенство базовых линий проверяется по числам базовой линии.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### См. также

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)



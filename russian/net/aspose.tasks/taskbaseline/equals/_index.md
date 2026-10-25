---
title: "TaskBaseline.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskBaseline. Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту TaskBaseline."
type: docs
weight: 100
url: /ru/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту `TaskBaseline`.

```csharp
public bool Equals(TaskBaseline other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | TaskBaseline | указанный объект AssignmentBaseline для сравнения с этим экземпляром. |

### Возвращаемое значение

возвращает true, если данный экземпляр равен указанному объекту TaskBaseline; иначе — false.

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

---

## Equals(object) {#equals_2}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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



---
title: "Task.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Task. Возвращает значение, указывающее, равен ли данный экземпляр указанной задаче."
type: docs
weight: 1330
url: /ru/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Возвращает значение, указывающее, равен ли этот экземпляр указанной задаче.

```csharp
public bool Equals(Task other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| другой | Задача | Указанная задача для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если указанная задача и этот экземпляр имеют одинаковые уникальные идентификаторы.

## Примеры

Показывает, как перебрать назначения задачи.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // отобразить назначения задачи
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Указанный объект для сравнения с этим экземпляром. |

### Возвращаемое значение

Возвращает true, если указанная задача и этот экземпляр имеют одинаковые уникальные идентификаторы.

## Примеры

Показывает, как перебрать назначения задачи.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // отобразить назначения задачи
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### См. также

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



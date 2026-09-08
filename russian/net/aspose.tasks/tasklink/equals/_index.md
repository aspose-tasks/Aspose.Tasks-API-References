---
title: "TaskLink.Equals"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод TaskLink. Возвращает значение, указывающее, равен ли данный экземпляр указанному объекту"
type: docs
weight: 90
url: /ru/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public bool Equals(TaskLink other)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| other | TaskLink | Указанный экземпляр класса [`TaskLink`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство ссылок задач.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Равенство ссылок задач основано на предшествующих и последующих задачах.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### См. также

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Объект | Объект для сравнения с этим экземпляром. |

### Возвращаемое значение

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Примеры

Показывает, как проверить равенство ссылок задач.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Равенство ссылок задач основано на предшествующих и последующих задачах.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### См. также

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)



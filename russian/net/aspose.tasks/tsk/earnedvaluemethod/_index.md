---
title: "Tsk.EarnedValueMethod"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, следует ли использовать поле Complete или Physical Complete для расчёта бюджетной стоимости выполненных работ (BCWP)."
type: docs
weight: 350
url: /ru/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

Определяет, следует ли использовать поле % Выполнено или Физический % Выполнено для расчёта запланированной стоимости выполненных работ (BCWP).

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.EarnedValueMethod.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



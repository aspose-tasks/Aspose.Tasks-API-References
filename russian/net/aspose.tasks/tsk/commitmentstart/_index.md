---
title: "Tsk.CommitmentStart"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата начала поставки. Чтение поддерживается только в формате XML"
type: docs
weight: 180
url: /ru/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

Дата начала поставки. Чтение поддерживается только для формата XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



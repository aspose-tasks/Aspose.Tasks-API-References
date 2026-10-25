---
title: "Tsk.CommitmentFinish"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Дата завершения поставки. Чтение поддерживается только в формате XML"
type: docs
weight: 170
url: /ru/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

Дата завершения поставки. Чтение поддерживается только для формата XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



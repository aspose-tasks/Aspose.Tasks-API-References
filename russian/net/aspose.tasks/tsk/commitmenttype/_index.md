---
title: "Tsk.CommitmentType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, имеет ли задача связанную поставку или зависимость от связанной поставки. Чтение поддерживается только в формате XML"
type: docs
weight: 190
url: /ru/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Определяет, имеет ли задача связанную поставку или зависимость от связанной поставки. Чтение поддерживается только для формата XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



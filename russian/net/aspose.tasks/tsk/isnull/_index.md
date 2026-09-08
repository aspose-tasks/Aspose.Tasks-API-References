---
title: "Tsk.IsNull"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача нулевой задачей"
type: docs
weight: 640
url: /ru/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

Определяет, является ли задача нулевой задачей.

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsNull.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



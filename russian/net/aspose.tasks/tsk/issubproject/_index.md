---
title: "Tsk.IsSubproject"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, является ли задача вставленным проектом"
type: docs
weight: 700
url: /ru/net/aspose.tasks/tsk/issubproject/
---
## Tsk.IsSubproject field

Определяет, является ли задача вставленным проектом.

```csharp
public static readonly Key<bool, TaskKey> IsSubproject;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsSubproject.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubproject, true);

Console.WriteLine("Is Subproject: " + task.Get(Tsk.IsSubproject));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



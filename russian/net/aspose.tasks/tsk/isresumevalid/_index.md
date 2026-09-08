---
title: "Tsk.IsResumeValid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, может ли задача быть возобновлена"
type: docs
weight: 680
url: /ru/net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Определяет, может ли задача быть возобновлена.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.IsResumeValid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



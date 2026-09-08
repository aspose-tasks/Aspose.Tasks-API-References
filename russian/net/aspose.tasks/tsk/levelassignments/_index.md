---
title: "Tsk.LevelAssignments"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Определяет, может ли функция выравнивания задерживать и разбивать отдельные назначения для устранения переизбыточных распределений"
type: docs
weight: 750
url: /ru/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Определяет, может ли функция выравнивания задерживать и разбивать отдельные назначения, чтобы решить проблему переизбыточных распределений.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.LevelAssignments.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



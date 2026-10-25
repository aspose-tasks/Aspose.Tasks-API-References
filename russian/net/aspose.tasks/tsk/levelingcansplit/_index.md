---
title: "Tsk.LevelingCanSplit"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Tsk field. Определяет, может ли функция выравнивания ресурсов вызывать разбиения оставшейся работы по этой задаче"
type: docs
weight: 760
url: /ru/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Определяет, может ли функция выравнивания ресурсов вызывать разбивку оставшейся работы по этой задаче.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Примеры

Показывает, как читать/записывать свойство Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



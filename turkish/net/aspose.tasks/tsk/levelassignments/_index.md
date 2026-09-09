---
title: "Tsk.LevelAssignments"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Dengeleme işlevinin aşırı tahsisleri çözmek için bireysel atamaları geciktirip bölüp bölmediğini belirler"
type: docs
weight: 750
url: /tr/net/aspose.tasks/tsk/levelassignments/
---
## Tsk.LevelAssignments field

Dengeleme işlevinin aşırı tahsisleri çözmek için bireysel atamaları geciktirip bölüp bölmeyeceğini belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelAssignments;
```

## Örnekler

Tsk.LevelAssignments özelliğinin nasıl okunup yazıldığını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelAssignments, true);

Console.WriteLine("Level Assignments: " + task.Get(Tsk.LevelAssignments));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



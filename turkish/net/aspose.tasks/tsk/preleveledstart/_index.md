---
title: "Tsk.PreleveledStart"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Kaynak dengelemesi yapılmadan önceki görev başlangıç tarihi"
type: docs
weight: 920
url: /tr/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

Kaynak dengelemesi yapılmadan önce bir görevin başlangıç tarihi.

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## Örnekler

Tsk.PreleveledStart özelliğinin nasıl okunup yazılacağını gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



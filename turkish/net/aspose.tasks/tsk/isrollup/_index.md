---
title: "Tsk.IsRollup"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Tsk alanı. Alt görev Gantt çubuklarıyla ilgili bilginin özet görev çubuğuna toplanıp toplanmayacağını belirler."
type: docs
weight: 690
url: /tr/net/aspose.tasks/tsk/isrollup/
---
## Tsk.IsRollup field

Alt görev Gantt çubuklarıyla ilgili bilginin özet görev çubuğuna yansıtılıp yansıtılmayacağını belirler.

```csharp
public static readonly Key<NullableBool, TaskKey> IsRollup;
```

## Örnekler

Tsk.IsRollup özelliğini okuma/yazma nasıl yapılır gösterir.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsRollup, true);

Console.WriteLine("Is Rollup: " + task.Get(Tsk.IsRollup));
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



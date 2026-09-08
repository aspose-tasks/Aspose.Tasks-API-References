---
title: "Tsk.Work"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De totale tijd die voor een taak is gepland voor alle toegewezen resources."
type: docs
weight: 1150
url: /nl/net/aspose.tasks/tsk/work/
---
## Tsk.Work field

De totale tijd die voor een taak is gepland voor alle toegewezen resources.

```csharp
public static readonly Key<Duration, TaskKey> Work;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.Work te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Work, project.GetWork(1));

Console.WriteLine("Work: " + task.Get(Tsk.Work));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



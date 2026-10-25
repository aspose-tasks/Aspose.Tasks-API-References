---
title: "Tsk.ActualWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De hoeveelheid werk die al is uitgevoerd door resources die aan taken zijn toegewezen"
type: docs
weight: 90
url: /nl/net/aspose.tasks/tsk/actualwork/
---
## Tsk.ActualWork field

De hoeveelheid werk die al is gedaan door resources die aan taken zijn toegewezen.

```csharp
public static readonly Key<Duration, TaskKey> ActualWork;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ActualWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + task.Get(Tsk.ActualWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



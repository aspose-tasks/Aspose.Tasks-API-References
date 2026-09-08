---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De werkelijke hoeveelheid overuren die al is uitgevoerd door aan taken toegewezen resources"
type: docs
weight: 60
url: /nl/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

De feitelijke hoeveelheid overuren die al door resources die aan taken zijn toegewezen, is uitgevoerd.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ActualOvertimeWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



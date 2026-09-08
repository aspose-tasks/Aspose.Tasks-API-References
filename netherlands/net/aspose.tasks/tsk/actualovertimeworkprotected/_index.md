---
title: "Tsk.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De duur gedurende welke daadwerkelijke overuren beschermd zijn"
type: docs
weight: 70
url: /nl/net/aspose.tasks/tsk/actualovertimeworkprotected/
---
## Tsk.ActualOvertimeWorkProtected field

De duur gedurende welke feitelijke overuren worden beschermd.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWorkProtected;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.ActualOvertimeWorkProtected gelezen/geschreven kan worden.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + task.Get(Tsk.ActualOvertimeWorkProtected));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



---
title: "Tsk.Duration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het totale bereik van actieve werktijd voor een taak, zoals ingevoerd of berekend door Microsoft Project op basis van startdatum, einddatum, agenda's en andere planningsfactoren."
type: docs
weight: 300
url: /nl/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

De totale duur van actieve werktijd voor een taak zoals ingevoerd of berekend door Microsoft Project op basis van startdatum, einddatum, agenda's en andere planningsfactoren.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Voorbeelden

Toont hoe de duur van de taak in te stellen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



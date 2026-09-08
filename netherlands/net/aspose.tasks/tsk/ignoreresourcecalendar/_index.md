---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Bepaalt of de planning van de taak rekening houdt met de agenda's van de aan de taak toegewezen resources"
type: docs
weight: 530
url: /nl/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Bepaalt of de planning van de taak rekening houdt met de agenda's van de aan de taak toegewezen resources.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.IgnoreResourceCalendar te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



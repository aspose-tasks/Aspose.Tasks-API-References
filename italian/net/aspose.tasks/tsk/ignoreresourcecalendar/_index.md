---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Determina se la programmazione dell'attività considera i calendari delle risorse assegnate all'attività"
type: docs
weight: 530
url: /it/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Determina se la pianificazione dell'attività considera i calendari delle risorse assegnate all'attività.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



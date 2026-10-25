---
title: "Tsk.Warning"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Geeft de vlag weer die aangeeft dat de taak planningsverschillen heeft"
type: docs
weight: 1120
url: /nl/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

Geeft weer de vlag die aangeeft dat een taak planningsverschillen heeft.

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## Voorbeelden

Toont hoe een taakwaarschuwing te lezen.

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



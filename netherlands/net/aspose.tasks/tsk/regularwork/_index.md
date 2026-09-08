---
title: "Tsk.RegularWork"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het totale aantal niet‑overurenwerk dat gepland is om door resources uitgevoerd te worden."
type: docs
weight: 940
url: /nl/net/aspose.tasks/tsk/regularwork/
---
## Tsk.RegularWork field

De totale hoeveelheid niet-overurenwerk die gepland is om door resources uitgevoerd te worden.

```csharp
public static readonly Key<Duration, TaskKey> RegularWork;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.RegularWork te lezen/schrijven.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + task.Get(Tsk.RegularWork));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



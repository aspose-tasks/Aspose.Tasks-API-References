---
title: "Tsk.EarlyFinish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De vroegste datum waarop een taak mogelijk kan eindigen, gebaseerd op vroegste einddatums van voorganger‑ en opvolger‑taken, andere beperkingen en eventuele level‑vertraging."
type: docs
weight: 330
url: /nl/net/aspose.tasks/tsk/earlyfinish/
---
## Tsk.EarlyFinish field

De vroegste datum waarop een taak mogelijk kan eindigen, gebaseerd op vroege einddatums van voorganger- en opvolgtaak, andere beperkingen en eventuele nivelleringvertraging.

```csharp
public static readonly Key<DateTime, TaskKey> EarlyFinish;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.EarlyFinish te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarlyFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Early Finish: " + task.Get(Tsk.EarlyFinish));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



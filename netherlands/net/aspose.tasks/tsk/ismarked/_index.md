---
title: "Tsk.IsMarked"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. Toont of een taak gemarkeerd is voor verdere actie of identificatie van een bepaald type"
type: docs
weight: 620
url: /nl/net/aspose.tasks/tsk/ismarked/
---
## Tsk.IsMarked field

Toont of een taak gemarkeerd is voor verdere actie of een bepaalde identificatie.

```csharp
public static readonly Key<bool, TaskKey> IsMarked;
```

## Opmerkingen

Alleen van toepassing op het mpp-bestandsformaat.

## Voorbeelden

Toont hoe de Tsk.IsMarked eigenschap gelezen/geschreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsMarked, true);

Console.WriteLine("Is Marked: " + task.Get(Tsk.IsMarked));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



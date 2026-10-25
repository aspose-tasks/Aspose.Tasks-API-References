---
title: "Tsk.Created"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De datum waarop een taak is aangemaakt"
type: docs
weight: 250
url: /nl/net/aspose.tasks/tsk/created/
---
## Tsk.Created field

De datum waarop een taak is aangemaakt.

```csharp
public static readonly Key<DateTime, TaskKey> Created;
```

## Voorbeelden

Toont hoe de Tsk.Created-eigenschap gelezen/schreven kan worden.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + task.Get(Tsk.Created));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



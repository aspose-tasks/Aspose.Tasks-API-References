---
title: "Tsk.Guid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. De gegenereerde unieke identificatiecodes voor een taak"
type: docs
weight: 460
url: /nl/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

De gegenereerde unieke identificatiecodes voor een taak.

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## Voorbeelden

Toont hoe de eigenschap Tsk.Guid te lezen/schrijven.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)



---
title: "Prj.NewTasksAreManual"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. Bepaalt of nieuwe taken handmatig worden aangemaakt"
type: docs
weight: 550
url: /nl/net/aspose.tasks/prj/newtasksaremanual/
---
## Prj.NewTasksAreManual field

Bepaalt of nieuwe taken handmatig worden aangemaakt.

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksAreManual;
```

## Voorbeelden

Toont hoe de eigenschap Prj.NewTasksAreManual te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.NewTasksAreManual, true);

Console.WriteLine("New Tasks Are Manual: " + project.Get(Prj.NewTasksAreManual));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



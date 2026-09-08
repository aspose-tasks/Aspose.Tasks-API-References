---
title: "Prj.ActualsInSync"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of al het werkelijke werk is gesynchroniseerd met het project"
type: docs
weight: 10
url: /nl/net/aspose.tasks/prj/actualsinsync/
---
## Prj.ActualsInSync field

Bepaalt of al het werk daadwerkelijk is gesynchroniseerd met het project.

```csharp
public static readonly Key<NullableBool, PrjKey> ActualsInSync;
```

## Voorbeelden

Toont hoe de eigenschap Prj.ActualsInSync gelezen/geschreven kan worden.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



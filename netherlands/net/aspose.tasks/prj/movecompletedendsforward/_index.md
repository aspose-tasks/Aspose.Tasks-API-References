---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of het einde van voltooide delen van taken die gepland waren om vóór de statusdatum te zijn voltooid maar later zijn begonnen, moet worden verplaatst naar de statusdatum"
type: docs
weight: 500
url: /nl/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

Bepaalt of het einde van voltooide delen van taken die gepland stonden om vóór de statusdatum te zijn voltooid maar later begonnen zijn, moet worden verplaatst naar de statusdatum.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## Voorbeelden

Toont hoe de eigenschap Prj.MoveCompletedEndsForward te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



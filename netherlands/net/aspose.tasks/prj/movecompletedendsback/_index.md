---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of het einde van voltooide delen van taken die gepland zijn om te starten na de statusdatum, maar eerder zijn gestart, moet worden teruggeplaatst naar de statusdatum"
type: docs
weight: 490
url: /nl/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

Bepaalt of het einde van voltooide delen van taken die gepland staan om na de statusdatum te starten maar eerder begonnen zijn, moet worden teruggezet naar de statusdatum.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## Voorbeelden

Toont hoe de eigenschap Prj.MoveCompletedEndsBack te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



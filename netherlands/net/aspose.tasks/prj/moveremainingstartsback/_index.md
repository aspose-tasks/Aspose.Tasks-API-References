---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Bepaalt of het begin van resterende delen van taken die gepland zijn om te starten na de statusdatum, maar eerder zijn gestart, moet worden teruggeplaatst naar de statusdatum."
type: docs
weight: 510
url: /nl/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

Bepaalt of het begin van de resterende delen van taken die gepland zijn om na de statusdatum te starten, maar eerder zijn gestart, moet worden teruggezet naar de statusdatum.

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## Voorbeelden

Toont hoe de eigenschap Prj.MoveRemainingStartsBack te lezen/schrijven.

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



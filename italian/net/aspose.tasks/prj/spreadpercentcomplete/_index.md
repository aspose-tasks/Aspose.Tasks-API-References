---
title: "Prj.SpreadPercentComplete"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Determina se una percentuale completata è distribuita alla data di stato"
type: docs
weight: 670
url: /it/net/aspose.tasks/prj/spreadpercentcomplete/
---
## Prj.SpreadPercentComplete field

Determina se la percentuale di completamento viene distribuita fino alla data di stato.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadPercentComplete;
```

## Esempi

Mostra come leggere/scrivere la proprietà Prj.SpreadPercentComplete.

```csharp
var project = new Project();

project.Set(Prj.SpreadPercentComplete, true);

Console.WriteLine("Spread Percent Complete: " + project.Get(Prj.SpreadPercentComplete));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)



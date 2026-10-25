---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraSaveOptions eigenschap. Haalt een waarde op of stelt een waarde in die aangeeft of activiteit-ID's moeten worden genummerd"
type: docs
weight: 50
url: /nl/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Haalt op of stelt een waarde in die aangeeft of activiteit-ID's moeten worden hergenummerd.

```csharp
public bool RenumberActivityIds { get; set; }
```

## Voorbeelden

Toont hoe te werken met &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// maak Primavera opslaanopties en stem ze af
var options = new PrimaveraSaveOptions
                  {
                      // definieer voorvoegsel en achtervoegsel van een activiteit
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // beheers het hernummeren van activiteiten
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Zie ook

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)



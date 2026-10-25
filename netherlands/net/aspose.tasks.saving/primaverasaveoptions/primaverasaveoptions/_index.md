---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraSaveOptions constructor. Initialiseert een nieuw exemplaar van de PrimaveraSaveOptions-klasse"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Initialiseert een nieuw exemplaar van de [`PrimaveraSaveOptions`](../) klasse.

```csharp
public PrimaveraSaveOptions()
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



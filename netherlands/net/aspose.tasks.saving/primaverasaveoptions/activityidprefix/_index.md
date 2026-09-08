---
title: "PrimaveraSaveOptions.ActivityIdPrefix"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrimaveraSaveOptions eigenschap. Haalt het voorvoegsel op of stelt het voorvoegsel in dat wordt gebruikt bij het hernummeren van activiteit-ID's"
type: docs
weight: 30
url: /nl/net/aspose.tasks.saving/primaverasaveoptions/activityidprefix/
---
## PrimaveraSaveOptions.ActivityIdPrefix property

Haalt op of stelt het voorvoegsel in dat wordt gebruikt bij het hernummeren van activiteit-ID's.

```csharp
public string ActivityIdPrefix { get; set; }
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



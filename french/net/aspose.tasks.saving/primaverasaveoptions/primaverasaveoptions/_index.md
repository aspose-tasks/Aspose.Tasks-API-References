---
title: "PrimaveraSaveOptions.PrimaveraSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PrimaveraSaveOptions. Initialise une nouvelle instance de la classe PrimaveraSaveOptions"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/primaverasaveoptions/primaverasaveoptions/
---
## PrimaveraSaveOptions constructor

Initialise une nouvelle instance de la classe [`PrimaveraSaveOptions`](../).

```csharp
public PrimaveraSaveOptions()
```

## Exemples

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// créez les options d'enregistrement Primavera et ajustez-les
var options = new PrimaveraSaveOptions
                  {
                      // définissez le préfixe et le suffixe d'une activité
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // contrôlez le renumérotage des activités
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Voir aussi

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)



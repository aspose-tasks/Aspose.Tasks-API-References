---
title: "PrimaveraSaveOptions.RenumberActivityIds"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraSaveOptions. Obtient ou définit une valeur indiquant s'il faut renuméroter les activity IDs"
type: docs
weight: 50
url: /fr/net/aspose.tasks.saving/primaverasaveoptions/renumberactivityids/
---
## PrimaveraSaveOptions.RenumberActivityIds property

Obtient ou définit une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité.

```csharp
public bool RenumberActivityIds { get; set; }
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



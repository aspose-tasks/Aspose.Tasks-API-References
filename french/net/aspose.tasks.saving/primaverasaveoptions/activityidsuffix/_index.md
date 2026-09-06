---
title: "PrimaveraSaveOptions.ActivityIdSuffix"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraSaveOptions. Obtient ou définit le suffixe utilisé lors du renumérotage des ID d'activité"
type: docs
weight: 40
url: /fr/net/aspose.tasks.saving/primaverasaveoptions/activityidsuffix/
---
## PrimaveraSaveOptions.ActivityIdSuffix property

Obtient ou définit le suffixe utilisé lors du renumérotage des ID d'activité.

```csharp
public int ActivityIdSuffix { get; set; }
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



---
title: "SaveOptions.NonWorkingTimeColor"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit la couleur du temps non travaillé."
type: docs
weight: 110
url: /fr/net/aspose.tasks.saving/saveoptions/nonworkingtimecolor/
---
## SaveOptions.NonWorkingTimeColor property

Obtient ou définit la couleur du temps non travaillé.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

## Exemples

Montre comment définir une couleur personnalisée pour le temps non travaillé.

```csharp
var project = new Project(DataDir + "ReadCurrencyProperties.mpp");
SaveOptions options = new PdfSaveOptions { NonWorkingTimeColor = Color.LightGray };
project.Save(OutDir + "ReadCurrencyProperties_out.pdf", options);
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)



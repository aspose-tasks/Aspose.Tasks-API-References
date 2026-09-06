---
title: "SaveOptions.FitContent"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu"
type: docs
weight: 50
url: /fr/net/aspose.tasks.saving/saveoptions/fitcontent/
---
## SaveOptions.FitContent property

Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu.

```csharp
public bool FitContent { get; set; }
```

## Exemples

Montre comment définir l'option indiquant si la hauteur de ligne doit être augmentée pour s'adapter à son contenu.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Définir l'option ajuster le contenu sur true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)



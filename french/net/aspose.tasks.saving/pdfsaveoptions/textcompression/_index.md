---
title: "PdfSaveOptions.TextCompression"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit un type de compression à utiliser pour tous les flux de contenu sauf les images. La valeur par défaut est Flate"
type: docs
weight: 100
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/textcompression/
---
## PdfSaveOptions.TextCompression property

Obtient ou définit le type de compression à utiliser pour tous les flux de contenu sauf les images. La valeur par défaut est Flate.

```csharp
public PdfTextCompression TextCompression { get; set; }
```

## Exemples

Montre comment définir un type de compression à utiliser pour tous les flux de contenu sauf les images.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// définir le type de compression à utiliser pour tous les flux de contenu sauf les images
options.TextCompression = PdfTextCompression.Flate;

// ajuster les propriétés supplémentaires
// définir le <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> dans lequel le document sera enregistré.
options.PresentationFormat = PresentationFormat.GanttChart;

// définir le niveau de conformité souhaité pour le document PDF généré
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithTextCompression_out.pdf", options);
```

### Voir aussi

* enum [PdfTextCompression](../../pdftextcompression/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)



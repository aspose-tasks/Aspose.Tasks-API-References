---
title: "Enumération PdfTextCompression"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enumération Aspose.Tasks.Saving.PdfTextCompression. Spécifie un type de compression appliqué à tout le contenu du fichier PDF sauf les images."
type: docs
weight: 2140
url: /fr/net/aspose.tasks.saving/pdftextcompression/
---
## PdfTextCompression enumeration

Spécifie un type de compression appliqué à tout le contenu du fichier PDF, sauf les images.

```csharp
public enum PdfTextCompression
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune compression. |
| Flate | `1` | Compression Flate. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)



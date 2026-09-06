---
title: "Enum PdfCompliance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PdfCompliance enum. Spécifie le niveau de conformité PDF du fichier de sortie"
type: docs
weight: 2070
url: /fr/net/aspose.tasks.saving/pdfcompliance/
---
## PdfCompliance enumeration

Spécifie le niveau de conformité PDF du fichier de sortie.

```csharp
public enum PdfCompliance
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Pdf15 | `0` | Niveau de conformité PDF/15. |
| PdfA1a | `1` | Niveau de conformité PDF/A-1a. |
| PdfA1b | `2` | Niveau de conformité PDF/A-1b. |

## Exemples

Montre comment définir un niveau de conformité souhaité pour le document PDF généré.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();

// définir le niveau de conformité souhaité pour le document PDF généré
// par défaut est le type <see cref=\"PdfCompliance.Pdf15\"/>
options.Compliance = PdfCompliance.PdfA1b;

// ajuster les propriétés supplémentaires
// définir le <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> dans lequel le document sera enregistré.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithPdfCompliance_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)



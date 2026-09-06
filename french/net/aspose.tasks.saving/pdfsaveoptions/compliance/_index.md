---
title: "PdfSaveOptions.Compliance"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit le niveau de conformité souhaité pour le document PDF généré. La valeur par défaut est Pdf15"
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Obtient ou définit le niveau de conformité souhaité pour le document PDF généré. La valeur par défaut est Pdf15.

```csharp
public PdfCompliance Compliance { get; set; }
```

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

* enum [PdfCompliance](../../pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)



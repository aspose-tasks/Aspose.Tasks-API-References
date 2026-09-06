---
title: "PdfSaveOptions.DigitalSignatureDetails"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit les détails d'une signature numérique. Si non défini, aucune signature ne sera effectuée"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/
---
## PdfSaveOptions.DigitalSignatureDetails property

Obtient ou définit les détails de la signature numérique. Si non défini, aucune signature ne sera effectuée.

```csharp
public PdfDigitalSignatureDetails DigitalSignatureDetails { get; set; }
```

## Exemples

Montre comment définir les détails d'une signature numérique. Si non défini, aucune signature ne sera effectuée.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions();
var certificate = new X509Certificate2();

// définir les détails d'une signature numérique. Si non défini, aucune signature ne sera effectuée.
options.DigitalSignatureDetails = new PdfDigitalSignatureDetails(
    certificate,
    "reason",
    "location",
    new DateTime(2019, 1, 1),
    PdfDigitalSignatureHashAlgorithm.Sha1);

// ajuster les propriétés supplémentaires
// définir le <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> dans lequel le document sera enregistré.
options.PresentationFormat = PresentationFormat.GanttChart;

// définir le niveau de conformité souhaité pour le document PDF généré
options.Compliance = PdfCompliance.PdfA1b;

project.Save(OutDir + "WorkWithDigitalSignatureDetails_out.pdf", options);
```

### Voir aussi

* class [PdfDigitalSignatureDetails](../../pdfdigitalsignaturedetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)



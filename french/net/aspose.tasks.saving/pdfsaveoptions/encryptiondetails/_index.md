---
title: "PdfSaveOptions.EncryptionDetails"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit les détails d'un chiffrement. Si non défini, aucun chiffrement ne sera effectué"
type: docs
weight: 40
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/encryptiondetails/
---
## PdfSaveOptions.EncryptionDetails property

Obtient ou définit les détails du chiffrement. Si non défini, aucun chiffrement ne sera effectué.

```csharp
public PdfEncryptionDetails EncryptionDetails { get; set; }
```

## Exemples

Montre comment définir les détails d'un chiffrement d'un document PDF. Si non défini, aucun chiffrement ne sera effectué.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var encryptionDetails = new PdfEncryptionDetails("userPassword", "ownerPassword", PdfEncryptionAlgorithm.RC4_128);

var options = new PdfSaveOptions();

// définir les détails d'un chiffrement d'un document PDF
options.EncryptionDetails = encryptionDetails;

// ajuster les propriétés supplémentaires
// définir le <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> dans lequel le document sera enregistré.
options.PresentationFormat = PresentationFormat.GanttChart;

project.Save(OutDir + "WorkWithEncryptionDetails_out.pdf", options);
```

### Voir aussi

* class [PdfEncryptionDetails](../../pdfencryptiondetails/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)



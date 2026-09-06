---
title: "PdfSaveOptions.PdfSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PdfSaveOptions. Initialise une nouvelle instance de la classe PdfSaveOptions qui peut être utilisée pour enregistrer un document au format PDF"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/pdfsaveoptions/
---
## PdfSaveOptions constructor

Initialise une nouvelle instance de la classe [`PdfSaveOptions`](../) qui peut être utilisée pour enregistrer un document au format [`PDF`](../../savefileformat/).

```csharp
public PdfSaveOptions()
```

## Exemples

Montre comment enregistrer les pages sélectionnées d'un projet dans un fichier PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// vérifions le nombre de pages pouvant être exportées
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Tasks](../../../)



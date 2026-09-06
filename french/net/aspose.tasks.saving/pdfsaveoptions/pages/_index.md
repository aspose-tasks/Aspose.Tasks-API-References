---
title: "PdfSaveOptions.Pages"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. Toutes les pages seront enregistrées si cette liste est vide"
type: docs
weight: 60
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/pages/
---
## PdfSaveOptions.Pages property

Obtient ou définit la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. Toutes les pages seront enregistrées si cette liste est vide.

```csharp
public List<int> Pages { get; set; }
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



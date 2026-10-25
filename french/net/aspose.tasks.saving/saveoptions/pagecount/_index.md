---
title: "SaveOptions.PageCount"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit le nombre de pages du projet"
type: docs
weight: 120
url: /fr/net/aspose.tasks.saving/saveoptions/pagecount/
---
## SaveOptions.PageCount property

Obtient ou définit le nombre de pages du projet.

```csharp
public int PageCount { get; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)



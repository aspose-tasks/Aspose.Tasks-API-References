---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur HtmlSaveOptions. Initialise une nouvelle instance de la classe HtmlSaveOptions"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions constructor

Initialise une nouvelle instance de la classe [`HtmlSaveOptions`](../).

```csharp
public HtmlSaveOptions()
```

## Exemples

Montre comment enregistrer un projet au format HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// OU

// Ajout d'une seule page (numéro de page 2)
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)



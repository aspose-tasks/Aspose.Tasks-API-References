---
title: "HtmlSaveOptions.IncludeProjectNameInTitle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML."
type: docs
weight: 120
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/
---
## HtmlSaveOptions.IncludeProjectNameInTitle property

Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML.

```csharp
public bool IncludeProjectNameInTitle { get; set; }
```

## Exemples

Montre comment définir l'en-tête/titre HTML de la page en utilisant les options &lt;see cref=\"P:Aspose.Tasks.Saving.HtmlSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new HtmlSaveOptions
{
    // Détermine s'il faut inclure le nom du projet dans le titre HTML (true par défaut)
    IncludeProjectNameInTitle = false,

    // Détermine s'il faut inclure le nom du projet dans l'en-tête de la page HTML (true par défaut)
    IncludeProjectNameInPageHeader = false,

    // définir les pages qui seront exportées
    Pages = new List<int>
            {
                1
            }
};
project.Save(OutDir + "ControlHeaderNameDuringHTMLExport_out.html", options);
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../htmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)



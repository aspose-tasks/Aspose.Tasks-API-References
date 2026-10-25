---
title: "HtmlSaveOptions.Pages"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété HtmlSaveOptions. Obtient ou définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. Toutes les pages du projet seront enregistrées si cette liste est vide"
type: docs
weight: 130
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/pages/
---
## HtmlSaveOptions.Pages property

Obtient ou définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. Toutes les pages du projet seront enregistrées si cette liste est vide.

```csharp
public List<int> Pages { get; set; }
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



---
title: "FontSettings.SetFontFolders"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode FontSettings. Définit les dossiers où Aspose.Tasks recherche les polices TrueType lors du rendu de la vue des projets"
type: docs
weight: 50
url: /fr/net/aspose.tasks/fontsettings/setfontfolders/
---
## FontSettings.SetFontFolders method

Définit les dossiers où Aspose.Tasks recherche les polices TrueType lors du rendu de la vue du projet.

```csharp
public void SetFontFolders(string[] fontFolders, bool recursive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fontFolders | String[] | Un tableau de dossiers contenant des polices TrueType. |
| recursive | Boolean | Si true, les dossiers spécifiés seront analysés de manière récursive. |

## Exemples

Montre comment définir un dossier de polices personnalisé.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

// Les fichiers de polices TrueType pour toutes les polices utilisées dans le projet ouvert doivent être situés dans le dossier MyFonts.
options.FontSettings.SetFontFolders(new string[] { "c:\\MyFonts"}, true);

project.Save(OutDir + "EstimatedMilestoneTasks_out4.pdf", options);
```

### Voir aussi

* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)



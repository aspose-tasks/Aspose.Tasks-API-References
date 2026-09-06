---
title: "SaveOptions.TextStyles"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit la liste des styles de texte appliqués lors du rendu d'une vue de projet."
type: docs
weight: 190
url: /fr/net/aspose.tasks.saving/saveoptions/textstyles/
---
## SaveOptions.TextStyles property

Obtient ou définit la liste des styles de texte appliqués lors du rendu d'une vue de projet.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Remarques

Ces styles remplacent les styles définis dans GanttCharView.TextStyles.

## Exemples

Montre comment utiliser les styles de texte des options d'enregistrement qui sont utilisés pour styliser différents éléments de texte dans un projet.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Bold | FontStyles.Italic)
{
    Color = Color.OrangeRed
};

style.ItemType = TextItemType.OverallocatedResources;

options.TextStyles = new List<TextStyle>
{
    style
};

project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Voir aussi

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)



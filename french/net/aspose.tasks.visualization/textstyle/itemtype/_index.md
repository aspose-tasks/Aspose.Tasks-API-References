---
title: "TextStyle.ItemType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TextStyle. Obtient ou définit le TextItemType du style de texte"
type: docs
weight: 60
url: /fr/net/aspose.tasks.visualization/textstyle/itemtype/
---
## TextStyle.ItemType property

Obtient ou définit le [`TextItemType`](../../textitemtype/) du style de texte.

```csharp
public virtual TextItemType ItemType { get; set; }
```

## Exemples

Montre comment personnaliser les styles de texte qui sont utilisés pour styliser différents éléments de texte dans un projet.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle();
style.Color = Color.OrangeRed;
style.Font = new FontDescriptor(FontFamily.GenericMonospace.Name, 10F, FontStyles.Bold | FontStyles.Italic);
style.ItemType = TextItemType.OverallocatedResources;
style.BackgroundColor = Color.Aqua;
style.BackgroundPattern = BackgroundPattern.DarkDither;

options.TextStyles = new List<TextStyle>
{
    style
};
project.Save(OutDir + "CustomizeTextStyle_out.pdf", options);
```

### Voir aussi

* enum [TextItemType](../../textitemtype/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



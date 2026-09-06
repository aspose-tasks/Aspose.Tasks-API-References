---
title: "TextStyle.Color"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TextStyle. Obtient ou définit la couleur du texte"
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/textstyle/color/
---
## TextStyle.Color property

Obtient ou définit la couleur du texte.

```csharp
public Color Color { get; set; }
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

* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



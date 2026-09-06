---
title: "TextStyle.Font"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TextStyle. Obtient ou définit la police du style de texte"
type: docs
weight: 50
url: /fr/net/aspose.tasks.visualization/textstyle/font/
---
## TextStyle.Font property

Obtient ou définit la police du style de texte.

```csharp
public FontDescriptor Font { get; set; }
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

* class [FontDescriptor](../../fontdescriptor/)
* class [TextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../textstyle/)
* assembly [Aspose.Tasks](../../../)



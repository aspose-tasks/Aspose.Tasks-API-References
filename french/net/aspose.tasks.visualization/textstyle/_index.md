---
title: "Classe TextStyle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.TextStyle. Modifiez le style visuel du texte pour un élément dans la vue du projet"
type: docs
weight: 3420
url: /fr/net/aspose.tasks.visualization/textstyle/
---
## TextStyle class

Modifiez le style visuel du texte pour un élément dans la vue du projet.

```csharp
public class TextStyle
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TextStyle](textstyle/#constructor)() | Initialise une nouvelle instance de la classe `TextStyle` avec les paramètres par défaut. |
| [TextStyle](textstyle/#constructor_1)(FontDescriptor) | Initialise une nouvelle instance de la classe `TextStyle` avec les paramètres de police spécifiés. |
| [TextStyle](textstyle/#constructor_2)(FontStyles) | Initialise une nouvelle instance de la classe `TextStyle` avec la police par défaut et le style de police spécifié. |
| [TextStyle](textstyle/#constructor_3)(float, FontStyles) | Initialise une nouvelle instance de la classe `TextStyle` avec la police par défaut et la taille et le style de police spécifiés. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du style de texte. [`Color`](./color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Obtient ou définit le motif d'arrière-plan du style de texte. [`BackgroundPattern`](./backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Obtient ou définit la couleur du texte. |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Obtient ou définit la police du style de texte. |
| virtual [ItemType](../../aspose.tasks.visualization/textstyle/itemtype/) { get; set; } | Obtient ou définit le [`TextItemType`](../textitemtype/) du style de texte. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



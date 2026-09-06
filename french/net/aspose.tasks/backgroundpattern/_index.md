---
title: "Enum BackgroundPattern"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.BackgroundPattern. Spécifie le motif d'arrière-plan"
type: docs
weight: 100
url: /fr/net/aspose.tasks/backgroundpattern/
---
## BackgroundPattern enumeration

Spécifie le motif d’arrière-plan.

```csharp
public enum BackgroundPattern
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DarkDiagonalLeft | `7` | Indique le motif d'arrière-plan diagonal sombre à gauche. |
| DarkDiagonalRight | `8` | Indique le motif d'arrière-plan diagonal sombre à droite. |
| DarkDither | `13` | Indique le motif d'arrière-plan à tramage sombre. |
| DarkFill | `4` | Indique le motif d'arrière-plan remplissage sombre. |
| DiagonalLeft | `5` | Indique le motif de fond diagonal gauche. |
| DiagonalRight | `6` | Indique le motif de fond diagonal droit. |
| Hollow | `0` | Indique le motif de fond creux. |
| LightDither | `11` | Indique le motif de fond à tramage léger. |
| LightFill | `2` | Indique le motif de fond à remplissage léger. |
| MediumDither | `12` | Indique le motif de fond à tramage moyen. |
| MediumFill | `3` | Indique le motif de fond à remplissage moyen. |
| MediumVerticalStripe | `10` | Indique le motif de fond à bandes verticales moyennes. |
| SolidFill | `1` | Indique le motif de fond à remplissage plein. |
| ThinVerticalStripe | `9` | Indique le motif de fond à bandes verticales fines. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



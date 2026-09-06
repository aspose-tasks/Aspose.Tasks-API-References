---
title: "Énumération TextItemType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.Visualization.TextItemType. Type d'élément pour changer un style de texte"
type: docs
weight: 3410
url: /fr/net/aspose.tasks.visualization/textitemtype/
---
## TextItemType enumeration

Type d'élément pour modifier un style de texte.

```csharp
public enum TextItemType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| RowColumnTitles | `0` | Titres des lignes et des colonnes. |
| CriticalTasks | `1` | Tâches critiques. |
| NoncriticalTasks | `2` | Tâches non critiques. |
| MilestoneTasks | `3` | Tâches jalons. |
| InactiveTasks | `4` | Tâches inactives. |
| SummaryTasks | `5` | Tâches de synthèse. |
| AssignmentRow | `6` | Ligne d'affectation. |
| TopTimescaleTier | `7` | Niveau supérieur de l'échelle de temps. |
| BottomTimescaleTier | `8` | Niveau inférieur de l'échelle de temps. |
| MiddleTimescaleTier | `9` | Niveau intermédiaire de l'échelle de temps. |
| Resources | `10` | Feuille de ressources. |
| OverallocatedResources | `11` | Ressources sur-allouées. |
| TaskFilterHighlight | `12` | Élément texte de mise en surbrillance du filtre de tâche. |
| BarTextBottom | `13` | Élément texte bas de la barre. |
| BarTextInside | `14` | Élément texte à l'intérieur de la barre. |
| BarTextLeft | `15` | Élément texte gauche de la barre. |
| BarTextRight | `16` | Élément texte droite de la barre. |
| BarTextTop | `17` | Élément texte haut de la barre. |
| MarkedTasks | `18` | Élément texte de tâche marquée. |
| ProjectSummary | `19` | Élément texte de tâche de synthèse du projet. |
| ExternalTasks | `20` | Élément texte de tâches externes. |
| Allocated | `21` | Élément texte alloué. |
| ChangedCells | `22` | Cellules modifiées. |

## Exemples

Montre comment travailler avec les types d'éléments texte.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.ResourceSheet
};

var style = new TextStyle(FontStyles.Italic | FontStyles.Bold)
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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



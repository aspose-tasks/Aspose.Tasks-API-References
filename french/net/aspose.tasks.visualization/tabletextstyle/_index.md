---
title: "Classe TableTextStyle"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.TableTextStyle. Représente un style de texte dans une table de vue"
type: docs
weight: 3370
url: /fr/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Représente un style de texte dans un tableau de vue.

```csharp
public class TableTextStyle : TextStyle
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Initialise une nouvelle instance de la classe `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Initialise une nouvelle instance de la classe `TableTextStyle` avec la police spécifiée. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Initialise une nouvelle instance de la classe `TableTextStyle` avec les paramètres de police par défaut et le style de police spécifié. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Initialise une nouvelle instance de la classe `TableTextStyle` avec la taille de police et le style de police spécifiés. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du style de texte. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Obtient ou définit le motif d'arrière-plan du style de texte. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Obtient ou définit la couleur du texte. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Obtient ou définit le champ auquel le style doit être appliqué. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Obtient ou définit la police du style de texte. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Renvoie une valeur de l'énumération [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Obtient un identifiant unique de ligne. Retourne -1 si le style doit être appliqué à toutes les lignes d'une vue. |

## Exemples

Montre comment personnaliser les styles de texte de tableau qui sont utilisés pour styliser différents éléments de texte dans un projet.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// définir le style de texte du premier nom de tâche
var style1 = new TableTextStyle(1);
// définir un champ auquel le style doit être appliqué.
style1.Field = Field.TaskName;
// définir <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> du style de texte.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// définir la taille en points de la police du style de texte.

// définir le style de texte de la durée de la deuxième tâche
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // définir un indicateur indiquant que les données de vue doivent être écrites
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Voir aussi

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



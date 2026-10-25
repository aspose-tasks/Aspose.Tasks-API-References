---
title: "TableTextStyle.RowUid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TableTextStyle. Obtient un identifiant unique de ligne. Retourne 1 si le style doit être appliqué à toutes les lignes d'une vue."
type: docs
weight: 40
url: /fr/net/aspose.tasks.visualization/tabletextstyle/rowuid/
---
## TableTextStyle.RowUid property

Obtient un identifiant unique de ligne. Retourne -1 si le style doit être appliqué à toutes les lignes d'une vue.

```csharp
public int RowUid { get; }
```

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

* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)



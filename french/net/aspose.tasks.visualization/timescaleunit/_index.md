---
title: "Enum TimescaleUnit"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.TimescaleUnit enum. Spécifie l'unité de temps pour chaque niveau d'une échelle de temps dans un diagramme de Gantt ou une autre vue à phases temporelles."
type: docs
weight: 3460
url: /fr/net/aspose.tasks.visualization/timescaleunit/
---
## TimescaleUnit enumeration

Spécifie l'unité de temps pour chaque niveau d'une échelle de temps dans un diagramme de Gantt ou une autre vue à phases temporelles.

```csharp
public enum TimescaleUnit
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `-1` | Indique Aucun. Le niveau de l'échelle de temps est masqué. |
| Minutes | `0` | Indique l'unité de temps Minutes. |
| Hours | `1` | Indique l'unité de temps Heures. |
| Days | `2` | Indique l'unité de temps Jours. |
| Weeks | `3` | Indique l'unité de temps Semaines. |
| ThirdsOfMonths | `4` | Indique l'unité de temps Tiers de mois. |
| Months | `5` | Indique l'unité de temps Mois. |
| Quarters | `6` | Indique l'unité de temps Trimestres d'années. |
| HalfYears | `7` | Indique l'unité de temps Semestres. |
| Years | `8` | Indique l'unité de temps Années. |

## Exemples

Ajouter des liens de tâche

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// ajuster les niveaux de l'échelle de temps
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// ajuster le niveau supérieur

// définir le niveau supérieur de l'échelle de temps de la vue du diagramme de Gantt.
// définir l'unité d'échelle de temps <see cref=\"T:Aspose.Tasks.Visualization.TimescaleUnit\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier = new TimescaleTier();
// définir l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// définir le libellé de date <see cref=\"T:Aspose.Tasks.Visualization.DateLabel\" /> pour le niveau de l'échelle de temps.
view.MiddleTimescaleTier.Count = 1;
// définir comment aligner les libellés à l'intérieur de chaque période de temps du niveau (<see cref=\"T:System.Drawing.StringAlignment\" />).
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// définir comment aligner les étiquettes dans chaque période de temps du niveau (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// définir une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau.
view.MiddleTimescaleTier.ShowTicks = true;
// définir une valeur indiquant s'il faut baser les libellés du niveau sur l'exercice fiscal.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// ajouté pour une meilleure visualisation
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// personnaliser les dates du niveau intermédiaire
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Utilisez l'option 'Timescale.DefinedInView' pour rendre les échelles de temps en utilisant les paramètres d'échelle de temps définis dans la vue (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



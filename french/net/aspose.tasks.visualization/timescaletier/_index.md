---
title: "Classe Aspose.Tasks.Visualization.TimescaleTier. Représente un seul niveau de l'échelle de temps sur un diagramme de Gantt"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Initialise une nouvelle instance de la classe `TimescaleTier`."
type: docs
weight: 3450
url: /fr/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Représente un niveau unique de l'échelle de temps sur un diagramme de Gantt.

```csharp
public sealed class TimescaleTier
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Obtient ou définit comment aligner les libellés à l'intérieur de chaque période de temps du niveau ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Obtient ou définit comment aligner les libellés à l'intérieur de chaque période de temps du niveau ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Obtient ou définit l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau. La valeur par défaut est 1. |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Obtient ou définit une fonction de rappel pour gérer le rendu du repère de date dans ce niveau. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Obtient ou définit le libellé de date [`DateLabel`](../datelabel/) pour le niveau de l'échelle de temps. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Obtient ou définit le drapeau qui indique si les libellés de date doivent être rendus sur chaque page lorsqu'une période de temps s'étend sur plusieurs pages. Si la valeur est 'true', lorsque la période de temps s'étend sur plusieurs pages, les libellés de date pour la période sont rendus sur chaque page. Si la valeur est 'false', le libellé de date est rendu une seule fois selon la valeur de la propriété [`Alignment`](./alignment/). |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut afficher les marques de graduation qui séparent les périodes de temps dans le niveau. |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Obtient ou définit l'unité d'échelle de temps [`TimescaleUnit`](../timescaleunit/) pour le niveau de l'échelle de temps. La valeur par défaut est [`Days`](../timescaleunit/). |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut baser les libellés du niveau sur l'année fiscale. |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Montre comment personnaliser les libellés du niveau de l'échelle de temps. |

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



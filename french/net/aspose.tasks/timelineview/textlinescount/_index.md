---
title: "TimelineView.TextLinesCount"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TimelineView. Obtient ou définit une valeur indiquant le nombre de lignes utilisées pour afficher la tâche dans une chronologie"
type: docs
weight: 80
url: /fr/net/aspose.tasks/timelineview/textlinescount/
---
## TimelineView.TextLinesCount property

Obtient ou définit une valeur indiquant combien de lignes sont utilisées pour afficher les tâches dans une chronologie.

```csharp
public int TextLinesCount { get; set; }
```

## Exemples

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.TimelineView\" /&gt;.

```csharp
var project = new Project();

// initialiser une vue de chronologie
var view = new TimelineView();

// définir une valeur indiquant comment formater les dates dans la vue Timeline.
view.DateFormat = DateFormat.DateDddDd;
// définir une valeur indiquant s'il faut afficher les tâches qui se chevauchent sur plusieurs lignes.
view.DisplayOverlapped = true;
// définir une valeur indiquant s'il faut afficher le contrôle de panoramique et de zoom.
view.ShowPanZoom = true;
// définir une valeur indiquant s'il faut afficher l'échelle de temps.
view.ShowTimescale = true;
// définir une valeur indiquant s'il faut afficher une ligne représentant aujourd'hui.
view.ShowToday = true;
// définir une valeur indiquant combien de lignes sont utilisées pour afficher les tâches dans une chronologie.
view.TextLinesCount = 2;

// obtient une valeur indiquant s'il faut afficher les tâches qui se chevauchent sur plusieurs lignes.
Console.WriteLine("Show Dates: " + view.ShowDates);

// ajouter la vue au projet
project.Views.Add(view);

// ajouter des données de test au projet
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Voir aussi

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)



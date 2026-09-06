---
title: "Enum BarItemType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.BarItemType enum. Type d'élément pour changer le style d'une barre."
type: docs
weight: 2940
url: /fr/net/aspose.tasks.visualization/baritemtype/
---
## BarItemType enumeration

Type d'élément pour modifier le style d'une barre.

```csharp
public enum BarItemType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Task | `0` | Indique le type d'élément de barre de tâche. |
| Summary | `1` | Indique le type d'élément de barre de résumé. |
| ProjectSummary | `2` | Indique le type d'élément de barre de résumé du projet. |
| ManualTask | `3` | Indique le type d'élément de barre de tâche manuelle. |
| InactiveTask | `4` | Indique le type d'élément de barre de tâche inactive. |
| CriticalTask | `5` | Indique le type d'élément de barre de tâche critique. |
| Milestone | `6` | Indique le type d'élément de barre de jalon. |
| ManualSummary | `7` | Indique le type d'élément de barre de résumé manuel. |
| Split | `8` | Indique le type d'élément de barre fractionnée. |
| ExternalTasks | `9` | Indique le type d'élément de barre de tâches externes. |
| ExternalMilestone | `10` | Indique le type d'élément de barre de jalon externe. |
| Deadline | `11` | Indique le type d'élément de barre d'échéance. |
| Progress | `12` | Indique le type d'élément de barre de progression. |
| StartOnly | `13` | Indique le type d'élément de barre de démarrage uniquement. |
| FinishOnly | `14` | Indique le type d'élément de barre de fin uniquement. |
| DurationOnly | `15` | Indique le type d'élément de barre de durée uniquement. |
| InactiveMilestone | `16` | Indique le type d'élément de barre de jalon inactif. |
| InactiveSummary | `17` | Indique le type d'élément de barre de résumé inactif. |
| SummaryRollup | `18` | Type d'élément de barre de regroupement de résumé. |

## Exemples

Montre comment personnaliser les barres de tâches en utilisant &lt;see cref="Aspose.Tasks.Visualization.BarStyle" /&gt;s.

```csharp
var project = new Project();

var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

var task3 = project.RootTask.Children.Add("Task 3");
var rsc1 = project.Resources.Add("Resource 1");
var rsc2 = project.Resources.Add("Resource 2");
var rsc3 = project.Resources.Add("Resource 3");

project.ResourceAssignments.Add(task1, rsc1);
project.ResourceAssignments.Add(task2, rsc2);
project.ResourceAssignments.Add(task3, rsc3);

SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.ThirdsOfMonths
};

var style = new BarStyle
                {
                    ItemType = BarItemType.CriticalTask,
                    LeftBarTextConverter = delegate(Task t)
                    {
                        return string.Format("This task (ID = {0}) is on critical path", t.Get(Tsk.Id));
                    }
                };

var style2 = new BarStyle { BarColor = Color.DarkOrchid, ItemType = BarItemType.Task };

options.BarStyles = new List<BarStyle> { style, style2 };

project.Save(OutDir + "CustomizeTextWithTaskBars_out.pdf", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



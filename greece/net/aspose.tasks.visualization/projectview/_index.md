---
title: "Κλάση ProjectView"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.Visualization.ProjectView. Κλάση προβολής έργων."
type: docs
weight: 3300
url: /el/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Κλάση προβολής του έργου

```csharp
public class ProjectView
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `ProjectView`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Λαμβάνει τις στήλες προβολής έργου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Περιλαμβάνει στήλες Uid, όνομα εργασίας, όνομα πόρου, εργασία και διάρκεια ανάθεσης. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Περιλαμβάνει στήλες id, δείκτες, όνομα, διάρκεια, έναρξη και λήξη εργασίας. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Περιλαμβάνει στήλες Uid, όνομα πόρου, τύπο, ετικέτα υλικού, αρχικά, ομάδα, μέγιστες μονάδες, τυπική τιμή, τιμή υπερωρίας, κόστος ανά χρήση, συσσωμάτωση, βασικό ημερολόγιο και κώδικα πόρου. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Περιλαμβάνει στήλες Uid, name, start, finish και work resource. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Περιλαμβάνει στήλες εργασίας id, indicators, name, duration, start, finish, predecessors και resource names. |

## Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έργο με προβολή ανάθεσης.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Κλάση Gridline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.Gridline κλάση. Η οριζόντια ή κάθετη γραμμή που εμφανίζεται στην προβολή του έργου."
type: docs
weight: 3100
url: /el/net/aspose.tasks.visualization/gridline/
---
## Gridline class

Η οριζόντια ή κάθετη γραμμή που εμφανίζεται στην προβολή του έργου.

```csharp
public class Gridline
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Gridline](gridline/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `Gridline`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Λαμβάνει ή ορίζει το [`Color`](./color/) μιας γραμμής πλέγματος. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο της γραμμής πλέγματος ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Λαμβάνει ή ορίζει το [`LinePattern`](../linepattern/) μιας γραμμής πλέγματος. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Επιστρέφει μια σημαία που υποδεικνύει εάν αυτή η παρουσία είναι ίση με το καθορισμένο αντικείμενο. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης `Gridline`. |

## Παραδείγματα

Δείχνει πώς να εργάζεστε με γραμμές πλέγματος κατά την αποθήκευση σε οπτικές μορφές.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // ορίστε τον τύπο της γραμμής πλέγματος (<see cref="P:Aspose.Tasks.Visualization.Gridline.GridlineType" />).
    GridlineType = GridlineType.GanttRow, 
    // ορίστε το <see cref="T:Aspose.Tasks.Visualization.LinePattern" /> μιας γραμμής πλέγματος
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



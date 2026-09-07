---
title: "Enum GridlineType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.GridlineType enum. Τύπος γραμμής πλέγματος"
type: docs
weight: 3110
url: /el/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Τύπος γραμμής πλέγματος.

```csharp
public enum GridlineType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| GanttRow | `0` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής σειράς gantt. |
| TopTierColumn | `1` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής στήλης ανώτερου επιπέδου. |
| BottomTierColumn | `2` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής στήλης κατώτερου επιπέδου. |
| SheetRow | `3` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής σειράς φύλλου. |
| SheetColumn | `4` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής στήλης φύλλου. |
| UsageRow | `5` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής σειράς χρήσης. |
| UsageColumn | `6` | Δείχνει τη γραμμή πλέγματος τύπου γραμμής στήλης χρήσης. |
| GanttTitleVertical | `7` | Δείχνει τον κάθετο τύπο γραμμής πλέγματος τίτλου Gantt. |
| GanttTitleHorizontal | `8` | Δείχνει τον οριζόντιο τύπο γραμμής πλέγματος τίτλου Gantt. |
| BarRows | `9` | Δείχνει τον τύπο γραμμής πλέγματος σειρών μπάρας. |
| GanttProjectStart | `10` | Δείχνει τον τύπο γραμμής πλέγματος έναρξης έργου Gantt. |
| GanttProjectFinish | `11` | Δείχνει τον τύπο γραμμής πλέγματος λήξης έργου Gantt. |
| GanttStatusDate | `12` | Υποδεικνύει τον τύπο της γραμμής πλέγματος της ημερομηνίας κατάστασης του Gantt. |
| GanttCurrentDate | `13` | Υποδεικνύει τον τύπο της γραμμής πλέγματος της τρέχουσας ημερομηνίας του Gantt. |
| GanttPageBreaks | `14` | Υποδεικνύει τον τύπο της γραμμής πλέγματος των διακοπών σελίδας του Gantt. |
| MiddleTierColumn | `15` | Υποδεικνύει τη γραμμή πλέγματος του ενδιάμεσου επιπέδου στήλης. |

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



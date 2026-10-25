---
title: "Gridline.Gridline"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής Gridline. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης Gridline."
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`Gridline`](../).

```csharp
public Gridline()
```

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

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)



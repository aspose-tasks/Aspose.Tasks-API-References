---
title: "Gridline.Color"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Gridline. Λαμβάνει ή ορίζει το Color μιας γραμμής πλέγματος."
type: docs
weight: 20
url: /el/net/aspose.tasks.visualization/gridline/color/
---
## Gridline.Color property

Λαμβάνει ή ορίζει το `Color` μιας γραμμής πλέγματος.

```csharp
public Color Color { get; set; }
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



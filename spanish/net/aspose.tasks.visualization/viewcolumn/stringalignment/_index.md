---
title: "ViewColumn.StringAlignment"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad ViewColumn. Obtiene o establece la alineación del texto; puede ser uno de los valores de la enumeración HorizontalStringAlignment."
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/viewcolumn/stringalignment/
---
## ViewColumn.StringAlignment property

Obtiene o establece la alineación del texto (puede ser uno de los valores de la enumeración [`HorizontalStringAlignment`](../../horizontalstringalignment/)).

```csharp
public HorizontalStringAlignment StringAlignment { get; set; }
```

## Ejemplos

Muestra cómo establecer una alineación del texto en una columna (puede ser uno de los valores de la &lt;see cref=\"P:Aspose.Tasks.Visualization.ViewColumn.StringAlignment\" /&gt; enumeración).

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions();
options.Timescale = Timescale.Months;
options.View = ProjectView.GetDefaultGanttChartView();

var column1 = (GanttChartColumn)options.View.Columns[2];
column1.StringAlignment = HorizontalStringAlignment.Center;
var column2 = (GanttChartColumn)options.View.Columns[3];
column2.StringAlignment = HorizontalStringAlignment.Far;
var column3 = (GanttChartColumn)options.View.Columns[4];
column3.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_GanttChart_out.pdf", options);

options.PresentationFormat = PresentationFormat.ResourceSheet;
options.View = ProjectView.GetDefaultResourceSheetView();

var column4 = (ResourceViewColumn)options.View.Columns[2];
column4.StringAlignment = HorizontalStringAlignment.Center;
var column5 = (ResourceViewColumn)options.View.Columns[3];
column5.StringAlignment = HorizontalStringAlignment.Far;
var column6 = (ResourceViewColumn)options.View.Columns[4];
column6.StringAlignment = HorizontalStringAlignment.Far;

project.Save(OutDir + "AlignCellContents_ResourceSheet_out.pdf", options);
```

### Ver también

* enum [HorizontalStringAlignment](../../horizontalstringalignment/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)



---
title: "CsvOptions.View"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad CsvOptions. Obtiene o establece una lista de las columnas de vista GanttChartColumn para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas"
type: docs
weight: 60
url: /es/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Obtiene o establece una lista de las columnas de vista ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas.

```csharp
public ProjectView View { get; set; }
```

## Ejemplos

Muestra cómo usar &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; para tomar las columnas del diagrama de Gantt predeterminado y

```csharp
// guardarlas en un archivo CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### Ver también

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)



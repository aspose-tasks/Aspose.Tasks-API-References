---
title: "Clase CsvOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Saving.CsvOptions. Permite especificar opciones adicionales al guardar el proyecto en CSV."
type: docs
weight: 1980
url: /es/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Permite especificar opciones adicionales al guardar el proyecto en CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CsvOptions](csvoptions/)() | Inicializa una nueva instancia de la clase `CsvOptions` que puede usarse para guardar el proyecto en formato CSV. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Obtiene o establece una categoría de datos que se guardará. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Obtiene o establece una codificación con la que guardar el CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Obtiene o establece un valor que indica si se deben incluir encabezados o no (el valor predeterminado es TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtiene o establece el formato en el que se guardará el documento si se utiliza este objeto de opciones de guardado. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtiene o establece el comparador para ordenar tareas en el diagrama de Gantt y en el diagrama de hoja de tareas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtiene o establece la condición que se utiliza para filtrar las tareas renderizadas en los diagramas de Gantt, hoja de tareas y uso de tareas. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Obtiene o establece un delimitador de texto. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Obtiene o establece una lista de las columnas de vista ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) para guardar en formato XLSX. Si no se establece, se guardan las columnas predeterminadas. |

## Ejemplos

Muestra cómo usar &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; para guardar un proyecto como archivo CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)



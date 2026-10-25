---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método FieldHelper. Devuelve un título predeterminado del campo específico."
type: docs
weight: 10
url: /es/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Devuelve un título predeterminado del campo específico.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| campo | Campo | Campo para obtener un título predeterminado. |

### Valor devuelto

Un título predeterminado del campo específico si el campo puede mostrarse en la vista de MS Project, null en caso contrario.

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)



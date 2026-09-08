---
title: "Clase TableField"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.TableField. Representa un campo de una tabla en un proyecto"
type: docs
weight: 2340
url: /es/net/aspose.tasks/tablefield/
---
## TableField class

Representa un campo de una tabla en un proyecto.

```csharp
public class TableField
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TableField](tablefield/)() | Inicializa una nueva instancia de la clase `TableField`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Obtiene o establece la alineación de los datos en un campo de tabla. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Obtiene o establece la alineación del título en un campo de tabla. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Obtiene o establece el tipo de un campo de tabla. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Obtiene o establece el título del campo en una tabla. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Obtiene o establece el ancho en puntos de la columna del campo en una tabla. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Obtiene o establece un valor que indica si el encabezado de la columna de la tabla puede ajustarse a varias líneas, o si debe truncarse cuando supera el ancho de la columna. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Obtiene o establece un valor que indica si el texto de la columna puede ajustarse a varias líneas, o si debe truncarse cuando supera el ancho de la columna. Compatible con la versión MSP 2010 y posteriores. |

## Ejemplos

Muestra cómo trabajar con la vista del proyecto y agregar una columna a la vista predeterminada (que se muestra cuando se abre un archivo MPP en MS Project).

```csharp
// crear un proyecto vacío sin vistas
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modificar la vista predeterminada (es una vista de diagrama de Gantt).
// O puedes seleccionar la vista por nombre o mediante la pantalla de vista usando la colección project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// La bandera WriteViewData debe usarse para persistir las modificaciones de las propiedades de la vista.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Muestra cómo leer las tablas del proyecto.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// obtener la tabla
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// mostrar la información de todos los campos de la tabla
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



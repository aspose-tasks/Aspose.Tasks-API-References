---
title: "Clase AssignmentViewColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.AssignmentViewColumn. Clase de vista de proyectos"
type: docs
weight: 2930
url: /es/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Clase de vista del proyecto.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Inicializa una nueva instancia de la clase AssignmentViewColumn. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Campo de columna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtiene el nombre de la columna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtiene o establece la alineación del texto (puede ser uno de los valores de la enumeración [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtiene o establece la devolución de llamada que puede usarse para personalizar la apariencia de las celdas de la columna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtiene el ancho de la columna. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Convierte la asignación de recurso actual al texto de la columna. |

## Ejemplos

Muestra cómo agregar columnas para vistas de asignación.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### Ver también

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



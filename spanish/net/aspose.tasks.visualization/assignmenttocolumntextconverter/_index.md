---
title: "Delegado AssignmentToColumnTextConverter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Convertidor de cadena de datos ResourceAssignment a columnas"
type: docs
weight: 2920
url: /es/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Convertidor de datos ResourceAssignment a cadena de columna.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| asignación | ResourceAssignment | La asignación a convertir. |

### Valor devuelto

Datos de cadena para la columna.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



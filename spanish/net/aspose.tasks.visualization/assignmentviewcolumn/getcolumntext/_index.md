---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método AssignmentViewColumn. Convierte la asignación de recurso actual al texto de la columna"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Convierte la asignación de recurso actual al texto de la columna.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| asignación | ResourceAssignment | Asignación actual. |

### Valor devuelto

El texto de la columna.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)



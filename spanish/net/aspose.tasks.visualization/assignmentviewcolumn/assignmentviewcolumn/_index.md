---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor AssignmentViewColumn. Inicializa una nueva instancia de la clase AssignmentViewColumn"
type: docs
weight: 10
url: /es/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Inicializa una nueva instancia de la clase AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | Cadena | Nombre de la columna. |
| ancho | Int32 | Ancho de la columna en píxeles. |
| convertidor | AssignmentToColumnTextConverter | Convertidor de datos de asignación a texto de columna. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)



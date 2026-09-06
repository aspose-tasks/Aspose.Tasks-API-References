---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur AssignmentViewColumn. Initialise une nouvelle instance de la classe AssignmentViewColumn"
type: docs
weight: 10
url: /fr/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Initialise une nouvelle instance de la classe AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | Chaîne | Nom de la colonne. |
| largeur | Int32 | Largeur de la colonne en pixels. |
| convertisseur | AssignmentToColumnTextConverter | Convertisseur de données d'affectation en texte de colonne. |

## Exemples

Montre comment ajouter des colonnes pour les vues d'affectation.

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

### Voir aussi

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)



---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode AssignmentViewColumn. Convertit l'affectation de ressource actuelle en texte de colonne"
type: docs
weight: 30
url: /fr/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Convertit l'affectation de ressource actuelle en texte de colonne.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| affectation | ResourceAssignment | Affectation actuelle. |

### Valeur de retour

Le texte de la colonne.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)



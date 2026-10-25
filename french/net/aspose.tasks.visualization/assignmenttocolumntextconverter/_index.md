---
title: "Délégué AssignmentToColumnTextConverter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Convertisseur de chaîne de données ResourceAssignment vers colonnes"
type: docs
weight: 2920
url: /fr/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Convertisseur de données ResourceAssignment en chaîne de caractères de colonne.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| affectation | ResourceAssignment | L'affectation à convertir. |

### Valeur de retour

Données de chaîne pour la colonne.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



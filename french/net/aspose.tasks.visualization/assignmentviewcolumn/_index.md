---
title: "Classe AssignmentViewColumn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.AssignmentViewColumn. Classe de vue des projets"
type: docs
weight: 2930
url: /fr/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Classe de vue du projet.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Initialise une nouvelle instance de la classe AssignmentViewColumn. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Champ de colonne. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtient le nom de la colonne. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtient ou définit l'alignement du texte (peut être l'une des valeurs de l'énumération [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtient ou définit le rappel qui peut être utilisé pour personnaliser l'apparence des cellules de la colonne. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtient la largeur de la colonne. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Convertit l'affectation de ressource actuelle en texte de colonne. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Classe ResourceViewColumn"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.ResourceViewColumn. Classe de vue des projets utilisée dans la vue ResourceUsage et la vue ResourceSheet"
type: docs
weight: 3350
url: /fr/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Classe de vue du projet utilisée dans la vue ResourceUsage et la vue ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Initialise une nouvelle instance de la classe `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Initialise une nouvelle instance de la classe `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Initialise une nouvelle instance de la classe `ResourceViewColumn`. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Champ de colonne. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtient le nom de la colonne. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtient ou définit l'alignement du texte (peut être l'une des valeurs de l'énumération [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtient ou définit le rappel qui peut être utilisé pour personnaliser l'apparence des cellules de la colonne. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtient la largeur de la colonne. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Convertit la ressource actuelle en texte de colonne. |

## Exemples

Montre comment ajouter des colonnes de vue des ressources à exporter.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// itérer sur les colonnes
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Voir aussi

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



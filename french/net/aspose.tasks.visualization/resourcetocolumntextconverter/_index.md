---
title: "Délégué ResourceToColumnTextConverter"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Convertisseur de données des ressources en chaîne de colonnes"
type: docs
weight: 3340
url: /fr/net/aspose.tasks.visualization/resourcetocolumntextconverter/
---
## ResourceToColumnTextConverter delegate

Convertisseur de données de ressource en chaîne de colonne.

```csharp
public delegate string ResourceToColumnTextConverter(Resource resource);
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ressource | Ressource | Ressource actuelle. |

### Valeur de retour

Données de chaîne pour la colonne.

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

* class [Resource](../../aspose.tasks/resource/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Classe TableField"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TableField. Représente un champ d'une table dans un projet."
type: docs
weight: 2340
url: /fr/net/aspose.tasks/tablefield/
---
## TableField class

Représente un champ d'une table dans un projet.

```csharp
public class TableField
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TableField](tablefield/)() | Initialise une nouvelle instance de la classe `TableField`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Obtient ou définit l'alignement des données dans un champ de tableau. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Obtient ou définit l'alignement du titre dans un champ de tableau. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Obtient ou définit le type d'un champ de tableau. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Obtient ou définit le titre du champ dans un tableau. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Obtient ou définit la largeur en points de la colonne du champ dans un tableau. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Obtient ou définit une valeur indiquant si l'en-tête de colonne du tableau peut s'étendre sur plusieurs lignes, ou s'il doit être tronqué lorsqu'il dépasse la largeur de la colonne. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Obtient ou définit une valeur indiquant si le texte de la colonne peut s’enrouler sur plusieurs lignes, ou s’il doit être tronqué lorsqu’il dépasse la largeur de la colonne. Pris en charge à partir de la version MSP 2010 et suivantes. |

## Exemples

Montre comment travailler avec la vue du projet et ajouter une colonne à la vue par défaut (qui est affichée lorsque le fichier MPP est ouvert dans MS Project).

```csharp
// créer un projet vide sans vues
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifier la vue par défaut (c’est une vue de diagramme de Gantt).
// Ou vous pouvez sélectionner la vue par son nom ou via l’écran de vue en utilisant la collection project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Le drapeau WriteViewData doit être utilisé pour persister les modifications des propriétés de la vue.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Montre comment lire les tables du projet.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// obtenir la table
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// afficher les informations de tous les champs de la table
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



---
title: "Classe TableCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TableCollection. Contient une liste d'objets Table. Implémente l'interface ICollectionTable"
type: docs
weight: 2330
url: /fr/net/aspose.tasks/tablecollection/
---
## TableCollection class

Contient une liste d'objets [`Table`](../table/). Implémente l'interface ICollection&lt;Table&gt;.

```csharp
public class TableCollection : ICollection<Table>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Convertit une collection de tables en une liste d'objets [`Table`](../table/). |

## Exemples

Montre comment travailler avec les collections de tables.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// parcourir les tables
Console.WriteLine("Print tables of " + project.Get(Prj.Name) + " project.");
Console.WriteLine("Table count: " + project.Tables.Count);
foreach (var tbl in project.Tables)
{
    Console.WriteLine("Name: " + tbl.Name);

    Console.WriteLine("Fields:");

    foreach (var field in tbl.TableFields)
    {
        Console.WriteLine("    {0} - '{1}' - {2}", field.Field, field.Title, field.Width);
    }
}

// ajouter une nouvelle table
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// on peut vider la collection de deux manières
if (deleteOneByOne)
{
    // copier les tables dans le tableau et les supprimer une par une
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // ou on peut vider complètement une collection de tables
    project.Tables.Clear();
}

// la collection peut être convertie en une simple liste de tables
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Voir aussi

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



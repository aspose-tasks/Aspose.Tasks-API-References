---
title: "Classe TableFieldCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TableFieldCollection. Contient une liste d'objets TableField. Implémente l'interface IListTableField."
type: docs
weight: 2350
url: /fr/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Contient une liste d'objets [`TableField`](../tablefield/). Implémente l'interface IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Obtient le nombre d'éléments contenus dans cette collection. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Obtient une valeur indiquant si cette collection est en lecture seule ; sinon, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Ajoute l'élément spécifié à cette collection. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Supprime tous les éléments de cette collection. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Copie les éléments de cette collection dans le tableau spécifié, en commençant à l'index de tableau spécifié. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Détermine l'index de l'élément spécifié dans cette collection. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Insère l'élément spécifié à l'index spécifié. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Supprime la première occurrence d'un objet spécifique de cette collection. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Supprime un élément à l'index spécifié. |

## Exemples

Montre comment travailler avec les collections de champs de tableau.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // itérer sur les champs de tableau
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// ajouter un nouveau champ de tableau
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// insérer un nouveau champ à la position
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// modifions le nouveau champ de tableau en utilisant l'accès par indice
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// récemment nous pouvons supprimer le champ
table.TableFields.RemoveAt(idx);

// on peut vider la collection de deux manières
if (deleteOneByOne)
{
    // copier les champs de tableau dans le tableau et les supprimer un par un
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // ou on peut vider complètement une collection de champs de tableau
    table.TableFields.Clear();
}
```

### Voir aussi

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



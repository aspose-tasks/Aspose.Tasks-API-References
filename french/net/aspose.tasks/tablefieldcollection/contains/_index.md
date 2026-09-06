---
title: "TableFieldCollection.Contains"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "TableFieldCollection méthode. Retourne vrai si l'élément spécifié est trouvé dans cette collection, sinon faux"
type: docs
weight: 60
url: /fr/net/aspose.tasks/tablefieldcollection/contains/
---
## TableFieldCollection.Contains method

Renvoie true si l'élément spécifié est trouvé dans cette collection ; sinon, false.

```csharp
public bool Contains(TableField item)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| élément | TableField | l'élément spécifié à trouver. |

### Valeur de retour

true si l'élément spécifié est trouvé dans cette collection ; sinon, false.

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

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)



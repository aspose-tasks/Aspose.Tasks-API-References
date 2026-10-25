---
title: "TableFieldCollection.RemoveAt"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TableFieldCollection. Rimuove un elemento all'indice specificato"
type: docs
weight: 120
url: /it/net/aspose.tasks/tablefieldcollection/removeat/
---
## TableFieldCollection.RemoveAt method

Rimuove un elemento all'indice specificato.

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice basato su zero specificato per rimuovere un elemento. |

## Esempi

Mostra come lavorare con le collezioni di campi tabella.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // iterare sui campi della tabella
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// aggiungere un nuovo campo tabella
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// inserire un nuovo campo nella posizione
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// consente di modificare il nuovo campo tabella usando l'accesso per indice
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// di recente possiamo rimuovere il campo
table.TableFields.RemoveAt(idx);

// è possibile svuotare la collezione in due modi
if (deleteOneByOne)
{
    // copiare i campi tabella nell'array e cancellarli uno per uno
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // oppure è possibile svuotare completamente una collezione di campi tabella
    table.TableFields.Clear();
}
```

### Vedi anche

* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)



---
title: "Classe TableFieldCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TableFieldCollection. Contiene un elenco di oggetti TableField. Implementa l'interfaccia IListTableField"
type: docs
weight: 2350
url: /it/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Contiene un elenco di oggetti [`TableField`](../tablefield/). Implementa l'interfaccia IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Restituisce o imposta l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Determina l'indice dell'elemento specificato in questa collezione. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Inserisce l'elemento specificato all'indice specificato. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Rimuove un elemento all'indice specificato. |

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

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



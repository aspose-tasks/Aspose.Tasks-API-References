---
title: "Classe TableCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TableCollection. Contiene un elenco di oggetti Table. Implementa l'interfaccia ICollectionTable"
type: docs
weight: 2330
url: /it/net/aspose.tasks/tablecollection/
---
## TableCollection class

Contiene un elenco di oggetti [`Table`](../table/) . Implementa l'interfaccia ICollection&lt;Table&gt;.

```csharp
public class TableCollection : ICollection<Table>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Converte una collezione di tabelle in un elenco di oggetti [`Table`](../table/). |

## Esempi

Mostra come lavorare con le collezioni di tabelle.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// iterare sulle tabelle
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

// aggiungere una nuova tabella
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// è possibile svuotare la collezione in due modi
if (deleteOneByOne)
{
    // copiare le tabelle nell'array e cancellarle una alla volta
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // oppure è possibile svuotare completamente una collezione di tabelle
    project.Tables.Clear();
}

// la collezione può essere convertita in un semplice elenco di tabelle
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Vedi anche

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



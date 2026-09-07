---
title: "TableCollection.Remove"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TableCollection. Rimuove la prima occorrenza di un oggetto specifico da questa collezione"
type: docs
weight: 80
url: /it/net/aspose.tasks/tablecollection/remove/
---
## TableCollection.Remove method

Rimuove la prima occorrenza di un oggetto specifico da questa collezione.

```csharp
public bool Remove(Table item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | Table | l'oggetto specificato da rimuovere. |

### Valore di ritorno

true se l'oggetto specificato è stato rimosso con successo da questa collezione; altrimenti, false.

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

* class [Table](../../table/)
* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)



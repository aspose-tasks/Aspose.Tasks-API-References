---
title: "TableCollection.Clear"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TableCollection yöntemi. Bu koleksiyondaki tüm öğeleri kaldırır."
type: docs
weight: 40
url: /tr/net/aspose.tasks/tablecollection/clear/
---
## TableCollection.Clear method

Bu koleksiyondaki tüm öğeleri kaldırır.

```csharp
public void Clear()
```

## Örnekler

Tablo koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// tablolar üzerinde yineleme yap
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

// yeni bir tablo ekle
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// koleksiyonu iki şekilde temizleyebilirsiniz
if (deleteOneByOne)
{
    // tabloları diziye kopyalayın ve tek tek silin
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // ya da bir tablo koleksiyonunu tamamen temizleyebilirsiniz
    project.Tables.Clear();
}

// koleksiyon, basit bir tablo listesine dönüştürülebilir
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Ayrıca Bakınız

* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)



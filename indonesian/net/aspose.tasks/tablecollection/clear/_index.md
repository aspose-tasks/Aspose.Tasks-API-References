---
title: "TableCollection.Clear"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TableCollection. Menghapus semua item dari koleksi ini"
type: docs
weight: 40
url: /id/net/aspose.tasks/tablecollection/clear/
---
## TableCollection.Clear method

Menghapus semua item dari koleksi ini.

```csharp
public void Clear()
```

## Contoh

Menampilkan cara bekerja dengan koleksi tabel.

```csharp
var project = new Project(DataDir + "Project1.mpp");

Console.WriteLine("Is collection of tables read-only?: " + project.Tables.IsReadOnly);

// mengiterasi tabel
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

// tambahkan tabel baru
var tableToAdd = new Table
{
    Name = "New Table",
    ShowInMenu = true
};
project.Tables.Add(tableToAdd);

Console.WriteLine("The collection contains the new table?: " + project.Tables.Contains(tableToAdd));

// seseorang dapat membersihkan koleksi dengan dua cara
if (deleteOneByOne)
{
    // salin tabel ke dalam array dan hapus satu per satu
    var tables = new Table[project.Tables.Count];
    project.Tables.CopyTo(tables, 0);
    foreach (var table in tables)
    {
        project.Tables.Remove(table);
    }
}
else
{
    // atau seseorang dapat mengosongkan koleksi tabel sepenuhnya
    project.Tables.Clear();
}

// koleksi dapat dikonversi menjadi daftar tabel biasa
List<Table> list = project.Tables.ToList();
foreach (var table in list)
{
    Console.WriteLine("Name: " + table.Name);
}
```

### Lihat Juga

* class [TableCollection](../)
* namespace [Aspose.Tasks](../../tablecollection/)
* assembly [Aspose.Tasks](../../../)



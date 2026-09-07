---
title: "TableFieldCollection.Insert"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TableFieldCollection metode. Menyisipkan item yang ditentukan pada indeks yang ditentukan"
type: docs
weight: 100
url: /id/net/aspose.tasks/tablefieldcollection/insert/
---
## TableFieldCollection.Insert method

Menyisipkan item yang ditentukan pada indeks yang ditentukan.

```csharp
public void Insert(int index, TableField item)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | Int32 | indeks berbasis nol yang ditentukan di mana item harus disisipkan. |
| item | TableField | item yang ditentukan untuk disisipkan ke koleksi ini. |

## Contoh

Menampilkan cara bekerja dengan koleksi bidang tabel.

```csharp
var project = new Project(DataDir + "Project1.mpp");

foreach (var tbl in project.Tables)
{
    Console.WriteLine("Table name: " + tbl.Name);
    Console.WriteLine("Is collection of table fields read-only?: " + tbl.TableFields.IsReadOnly);

    // iterasi melalui bidang tabel
    Console.WriteLine("Print table fields of " + project.Get(Prj.Name) + " project.");
    Console.WriteLine("Table count: " + tbl.TableFields.Count);
    foreach (var fld in tbl.TableFields)
    {
        Console.WriteLine("Field Title: " + fld.Title);
        Console.WriteLine("Field Field: " + fld.Field);
        Console.WriteLine();
    }
}

// tambahkan bidang tabel baru
var table = project.Tables.ToList()[0];
var field = new TableField();
field.Title = "New Table Field";
table.TableFields.Add(field);

var field2 = new TableField();
field2.Title = "New Table Field 2";

// sisipkan bidang baru pada posisi tersebut
var idx = table.TableFields.IndexOf(field);
table.TableFields.Insert(idx, field2);

// mengedit bidang tabel baru dengan menggunakan akses indeks
table.TableFields[idx].WrapHeader = true;

Console.WriteLine("The collection contains the new table field?: " + table.TableFields.Contains(field));

// baru-baru ini kita dapat menghapus bidang.
table.TableFields.RemoveAt(idx);

// seseorang dapat membersihkan koleksi dengan dua cara
if (deleteOneByOne)
{
    // salin bidang tabel ke dalam array dan hapus satu per satu
    var tableFields = new TableField[table.TableFields.Count];
    table.TableFields.CopyTo(tableFields, 0);
    foreach (var fld in tableFields)
    {
        table.TableFields.Remove(fld);
    }
}
else
{
    // atau seseorang dapat mengosongkan koleksi bidang tabel sepenuhnya
    table.TableFields.Clear();
}
```

### Lihat Juga

* class [TableField](../../tablefield/)
* class [TableFieldCollection](../)
* namespace [Aspose.Tasks](../../tablefieldcollection/)
* assembly [Aspose.Tasks](../../../)



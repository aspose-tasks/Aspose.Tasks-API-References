---
title: "TableFieldCollection.CopyTo"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TableFieldCollection. Menyalin elemen-elemen koleksi ini ke array yang ditentukan mulai dari indeks array yang ditentukan"
type: docs
weight: 70
url: /id/net/aspose.tasks/tablefieldcollection/copyto/
---
## TableFieldCollection.CopyTo method

Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan.

```csharp
public void CopyTo(TableField[] array, int arrayIndex)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| array | `TableField[]` | array satu dimensi yang ditentukan untuk menyalin elemen ke |
| arrayIndex | Int32 | indeks berbasis nol dari array yang ditentukan di mana penyalinan dimulai. |

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



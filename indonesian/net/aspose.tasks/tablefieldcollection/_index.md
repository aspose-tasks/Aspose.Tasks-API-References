---
title: "Kelas TableFieldCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TableFieldCollection. Berisi daftar objek TableField. Mengimplementasikan antarmuka IListTableField"
type: docs
weight: 2350
url: /id/net/aspose.tasks/tablefieldcollection/
---
## TableFieldCollection class

Berisi daftar objek [`TableField`](../tablefield/) . Mengimplementasikan antarmuka IList&lt;TableField&gt;.

```csharp
public class TableFieldCollection : IList<TableField>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/tablefieldcollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/tablefieldcollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |
| [Item](../../aspose.tasks/tablefieldcollection/item/) { get; set; } | Mengembalikan atau mengatur elemen pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/tablefieldcollection/add/)(TableField) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/tablefieldcollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/tablefieldcollection/contains/)(TableField) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/tablefieldcollection/copyto/)(TableField[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/tablefieldcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [IndexOf](../../aspose.tasks/tablefieldcollection/indexof/)(TableField) | Menentukan indeks dari item yang ditentukan dalam koleksi ini. |
| [Insert](../../aspose.tasks/tablefieldcollection/insert/)(int, TableField) | Menyisipkan item yang ditentukan pada indeks yang ditentukan. |
| [Remove](../../aspose.tasks/tablefieldcollection/remove/)(TableField) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [RemoveAt](../../aspose.tasks/tablefieldcollection/removeat/)(int) | Menghapus sebuah item pada indeks yang ditentukan. |

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

* class [TableField](../tablefield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



---
title: "Kelas TableCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TableCollection. Berisi daftar objek Table. Mengimplementasikan antarmuka ICollectionTable."
type: docs
weight: 2330
url: /id/net/aspose.tasks/tablecollection/
---
## TableCollection class

Berisi daftar objek [`Table`](../table/) . Mengimplementasikan antarmuka ICollection&lt;Table&gt;.

```csharp
public class TableCollection : ICollection<Table>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/tablecollection/count/) { get; } | Mendapatkan jumlah elemen yang terdapat dalam koleksi ini. |
| [IsReadOnly](../../aspose.tasks/tablecollection/isreadonly/) { get; } | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca; jika tidak, false. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/tablecollection/add/)(Table) | Menambahkan item yang ditentukan ke koleksi ini. |
| [Clear](../../aspose.tasks/tablecollection/clear/)() | Menghapus semua item dari koleksi ini. |
| [Contains](../../aspose.tasks/tablecollection/contains/)(Table) | Mengembalikan true jika item yang ditentukan ditemukan dalam koleksi ini; jika tidak, false. |
| [CopyTo](../../aspose.tasks/tablecollection/copyto/)(Table[], int) | Menyalin elemen-elemen koleksi ini ke array yang ditentukan, mulai dari indeks array yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/tablecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/tablecollection/remove/)(Table) | Menghapus kemunculan pertama dari objek tertentu dari koleksi ini. |
| [ToList](../../aspose.tasks/tablecollection/tolist/)() | Mengonversi koleksi tabel menjadi daftar objek [`Table`](../table/). |

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

* class [Table](../table/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



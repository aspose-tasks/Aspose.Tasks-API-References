---
title: "Table.Table"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Table constructor. Initializes a new instance of the Table class"
type: docs
weight: 10
url: /id/net/aspose.tasks/table/table/
---
## Table constructor

Initializes a new instance of the [`Table`](../) class.

```csharp
public Table()
```

## Contoh

Menampilkan cara mendefinisikan tabel baru (digunakan untuk tampilan).

```csharp
var project = new Project(DataDir + "Project1.mpp");

// dapatkan tabel untuk diedit
var table = project.Tables.ToList()[0];
Console.WriteLine("Uid of the table: " + table.Uid);
Console.WriteLine("Name of the table: " + table.Name);
Console.WriteLine("Type of the table: " + table.TableType);

// sesuaikan beberapa properti
// atur nilai yang menunjukkan apakah tinggi baris header tabel dapat disesuaikan
table.AdjustHeaderRowHeight = true;

// atur format tanggal tabel.
table.DateFormat = DateFormat.DateDdMmYyyy;

// atur nilai yang menunjukkan apakah kolom pertama tabel terkunci atau dapat diedit
table.LockFirstColumn = true;

// atur tinggi baris dalam tabel, di mana tinggi baris adalah jumlah baris teks
table.RowHeight = 10;

// mengatur nilai yang menunjukkan apakah akan menampilkan antarmuka 'Add New Column'
table.ShowAddNewColumn = true;

// atur nilai yang menunjukkan apakah proyek menampilkan nama tabel dalam daftar drop-down Tables pada tab View di Ribbon
table.ShowInMenu = true;

// memungkinkan menyimpan tabel yang diperbarui
project.Save(OutDir + "WorkWithTable_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)



---
title: "Kelas Table"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Table. Mewakili sebuah tabel dalam Project."
type: docs
weight: 2320
url: /id/net/aspose.tasks/table/
---
## Table class

Mewakili tabel dalam Project

```csharp
public class Table
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Table](table/)() | Menginisialisasi sebuah instance baru dari kelas `Table`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AdjustHeaderRowHeight](../../aspose.tasks/table/adjustheaderrowheight/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tinggi baris header tabel dapat disesuaikan. |
| [DateFormat](../../aspose.tasks/table/dateformat/) { get; set; } | Mendapatkan atau mengatur format tanggal tabel. |
| [LockFirstColumn](../../aspose.tasks/table/lockfirstcolumn/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah kolom pertama tabel terkunci atau dapat diedit. |
| [Name](../../aspose.tasks/table/name/) { get; set; } | Mendapatkan atau mengatur nama objek Table. |
| [RowHeight](../../aspose.tasks/table/rowheight/) { get; set; } | Mendapatkan atau mengatur tinggi baris dalam tabel, di mana tinggi baris adalah jumlah baris teks. |
| [ShowAddNewColumn](../../aspose.tasks/table/showaddnewcolumn/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menampilkan antarmuka 'Add New Column'. Didukung oleh versi MSP 2010 dan yang lebih baru. |
| [ShowInMenu](../../aspose.tasks/table/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah proyek menampilkan nama tabel dalam daftar drop-down Tables pada tab View di Ribbon. |
| [TableFields](../../aspose.tasks/table/tablefields/) { get; } | Mendapatkan koleksi TableFields yang mewakili bidang-bidang dalam tabel. |
| [TableType](../../aspose.tasks/table/tabletype/) { get; set; } | Mendapatkan atau mengatur tipe tabel untuk tabel yang ditentukan. |
| [Uid](../../aspose.tasks/table/uid/) { get; } | Mendapatkan pengidentifikasi unik dari sebuah tabel. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/table/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/table/gethashcode/)() | Mengembalikan kode hash untuk Tabel ini. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



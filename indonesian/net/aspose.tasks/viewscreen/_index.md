---
title: "Enum ViewScreen"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.ViewScreen. Menentukan jenis layar untuk tampilan"
type: docs
weight: 2910
url: /id/net/aspose.tasks/viewscreen/
---
## ViewScreen enumeration

Menentukan jenis layar untuk tampilan.

```csharp
public enum ViewScreen
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Calendar | `13` | Tampilan Kalender. |
| Gantt | `1` | Tampilan Gantt. |
| NetworkDiagram | `2` | Tampilan Diagram Jaringan. |
| RelationshipDiagram | `3` | Tampilan Diagram Hubungan. |
| ResourceForm | `6` | Tampilan Formulir Sumber Daya. |
| ResourceGraph | `8` | Tampilan Grafik Sumber Daya. |
| ResourceNameForm | `12` | Tampilan Formulir Nama Sumber Daya. |
| ResourceSheet | `7` | Tampilan Lembar Sumber Daya. |
| ResourceUsage | `15` | Tampilan Penggunaan Sumber Daya. |
| TaskDetailsForm | `10` | Tampilan Formulir Detail Tugas. |
| TaskForm | `4` | Tampilan Formulir Tugas. |
| TaskNameForm | `11` | Tampilan Formulir Nama Tugas. |
| TaskSheet | `5` | Tampilan Lembar Tugas. |
| TaskUsage | `14` | Tampilan Penggunaan Tugas. |

## Contoh

Menampilkan cara bekerja dengan tampilan Project dan menambahkan kolom ke tampilan default (yang ditampilkan ketika file MPP dibuka di MS Project).

```csharp
// buat proyek kosong tanpa tampilan
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifikasi tampilan default (ini adalah tampilan diagram Gantt).
// Atau Anda dapat memilih tampilan berdasarkan nama atau melalui Layar Tampilan menggunakan koleksi project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Flag WriteViewData harus digunakan untuk menyimpan perubahan properti tampilan.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Menampilkan cara bekerja dengan tampilan MS Project.

```csharp
// buat proyek kosong tanpa tampilan
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// buat tampilan diagram Gantt standar
View view = new GanttChartView();

// atur beberapa properti tampilan
// atur nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views di Ribbon
view.ShowInMenu = true;
// atur nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk tampilan tunggal
view.HighlightFilter = true;

// penulisan properti berikut tidak didukung
// mengatur filter yang digunakan dalam tampilan tunggal
view.Filter = null;
// mengatur grup dari tampilan tunggal
view.Group = null;
// mengatur tabel dari tampilan tunggal
view.Table = null;

// mari sesuaikan beberapa pengaturan tampilan
// atur jumlah kolom pertama yang akan dicetak pada semua halaman
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// atur nilai yang menunjukkan apakah mencetak sejumlah kolom pertama yang ditentukan pada semua halaman
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// tambahkan tampilan ke proyek kami
project.Views.Add(view);

// Flag WriteViewData harus digunakan untuk mempertahankan modifikasi project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// mari periksa beberapa properti dari tampilan yang baru ditambahkan
// cetak pengidentifikasi unik dari sebuah tampilan
Console.WriteLine("View Uid: " + view.Uid);
// cetak tipe layar untuk tampilan tunggal
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



---
title: "View.Filter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti View. Mendapatkan atau mengatur filter yang digunakan dalam satu tampilan"
type: docs
weight: 20
url: /id/net/aspose.tasks/view/filter/
---
## View.Filter property

Mendapatkan atau mengatur filter yang digunakan dalam tampilan tunggal.

```csharp
public Filter Filter { get; set; }
```

## Contoh

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

* class [Filter](../../filter/)
* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)



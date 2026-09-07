---
title: "Kelas View"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.View. Mewakili tampilan dalam Project"
type: docs
weight: 2890
url: /id/net/aspose.tasks/view/
---
## View class

Mewakili tampilan dalam Project.

```csharp
public class View : IComparable<View>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [View](view/#constructor)() | Menginisialisasi instance baru dari kelas `View`. |
| [View](view/#constructor_1)(ViewScreen) | Menginisialisasi instance baru dari kelas `View`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Mendapatkan atau mengatur filter yang digunakan dalam tampilan tunggal. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Mendapatkan atau mengatur grup dari tampilan tunggal. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk tampilan tunggal. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Mendapatkan atau mengatur nama objek View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Mendapatkan instance dari kelas [`PageInfo`](./pageinfo/). Mewakili data pengaturan halaman yang ada dalam format file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Mendapatkan induk dari objek View. Hanya-baca [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Mendapatkan tipe layar untuk tampilan tunggal. Hanya-baca [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views pada Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Mendapatkan atau mengatur tabel dari tampilan tunggal. |
| [Type](../../aspose.tasks/view/type/) { get; } | Mendapatkan tipe item dalam tampilan tunggal, seperti tugas atau sumber daya. Hanya-baca [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Mendapatkan pengenal unik dari sebuah tampilan. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Mendapatkan koleksi objek yang mewakili penempatan dan tampilan [`OleObject`](../oleobject/) dalam tampilan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Membandingkan instance saat ini dengan objek lain dengan tipe yang sama dan mengembalikan integer yang menunjukkan apakah instance saat ini mendahului, mengikuti, atau berada pada posisi yang sama dalam urutan penyortiran dibandingkan objek lainnya. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Mengembalikan nilai kode hash untuk instance dari kelas [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih besar dari objek yang ditentukan. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih besar atau sama dengan objek yang ditentukan. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Kembalikan nilai yang menunjukkan apakah instance ini tidak sama dengan objek yang ditentukan. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih kecil dari objek yang ditentukan. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Kembalikan nilai yang menunjukkan apakah instance ini lebih kecil atau sama dengan objek yang ditentukan. |

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



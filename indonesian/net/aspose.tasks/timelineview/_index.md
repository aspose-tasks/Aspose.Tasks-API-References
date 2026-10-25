---
title: "Kelas TimelineView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TimelineView. Mewakili tampilan linimasa sebuah proyek"
type: docs
weight: 2580
url: /id/net/aspose.tasks/timelineview/
---
## TimelineView class

Mewakili tampilan garis waktu proyek.

```csharp
public class TimelineView : View
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TimelineView](timelineview/)() | Menginisialisasi instance baru dari kelas `TimelineView`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan cara memformat tanggal pada tampilan Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan tugas yang tumpang tindih pada beberapa baris. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Mendapatkan atau mengatur filter yang digunakan dalam tampilan tunggal. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Mendapatkan atau mengatur grup dari tampilan tunggal. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk tampilan tunggal. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Mendapatkan atau mengatur nama objek View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Mendapatkan sebuah instance dari kelas [`PageInfo`](../view/pageinfo/). Mewakili data pengaturan halaman yang terdapat dalam format file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Mendapatkan induk dari objek View. Hanya-baca [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Mendapatkan tipe layar untuk tampilan tunggal. Hanya-baca [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Mendapatkan nilai yang menunjukkan apakah menampilkan tanggal. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views pada Ribbon. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan kontrol pan dan zoom. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan skala waktu. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan garis yang mewakili hari ini. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Mendapatkan atau mengatur tabel dari tampilan tunggal. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan berapa banyak garis yang digunakan untuk menampilkan tugas dalam linimasa. |
| [Type](../../aspose.tasks/view/type/) { get; } | Mendapatkan tipe item dalam tampilan tunggal, seperti tugas atau sumber daya. Hanya-baca [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Mendapatkan pengenal unik dari sebuah tampilan. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Mendapatkan koleksi objek yang mewakili penempatan dan tampilan [`OleObject`](../oleobject/) dalam tampilan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Membandingkan instance saat ini dengan objek lain dengan tipe yang sama dan mengembalikan integer yang menunjukkan apakah instance saat ini mendahului, mengikuti, atau berada pada posisi yang sama dalam urutan penyortiran dibandingkan objek lainnya. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Mengembalikan nilai kode hash untuk instance dari kelas [`Resource`](../resource/). |

## Contoh

Menampilkan cara bekerja dengan &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// inisialisasi tampilan linimasa
var view = new TimelineView();

// atur nilai yang menunjukkan cara memformat tanggal pada tampilan Timeline.
view.DateFormat = DateFormat.DateDddDd;
// atur nilai yang menunjukkan apakah menampilkan tugas yang tumpang tindih pada beberapa baris.
view.DisplayOverlapped = true;
// atur nilai yang menunjukkan apakah menampilkan kontrol pan dan zoom.
view.ShowPanZoom = true;
// atur nilai yang menunjukkan apakah menampilkan skala waktu.
view.ShowTimescale = true;
// atur nilai yang menunjukkan apakah menampilkan garis yang mewakili hari ini.
view.ShowToday = true;
// atur nilai yang menunjukkan berapa banyak garis yang digunakan untuk menampilkan tugas dalam linimasa.
view.TextLinesCount = 2;

// mendapatkan nilai yang menunjukkan apakah menampilkan tugas yang tumpang tindih pada beberapa baris.
Console.WriteLine("Show Dates: " + view.ShowDates);

// tambahkan tampilan ke proyek
project.Views.Add(view);

// tambahkan beberapa data uji ke proyek
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



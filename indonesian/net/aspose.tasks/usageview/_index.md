---
title: "Kelas UsageView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.UsageView. Mewakili tampilan penggunaan dalam sebuah proyek"
type: docs
weight: 2650
url: /id/net/aspose.tasks/usageview/
---
## UsageView class

Mewakili tampilan penggunaan dalam proyek.

```csharp
public abstract class UsageView : View
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Mendapatkan atau mengatur perataan data detail. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Mendapatkan atau mengatur pengaturan tingkat timescale bawah tampilan. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan kolom header detail dalam tampilan atau tidak. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan nama header detail singkat atau tidak. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Mendapatkan atau mengatur filter yang digunakan dalam tampilan tunggal. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Mendapatkan atau mengatur grup dari tampilan tunggal. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menyorot filter untuk tampilan tunggal. |
| [MiddleTimescaleTier](../../aspose.tasks/usageview/middletimescaletier/) { get; set; } | Mendapatkan atau mengatur pengaturan tingkat timescale tengah tampilan. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Mendapatkan atau mengatur nama objek View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Mendapatkan sebuah instance dari kelas [`PageInfo`](../view/pageinfo/). Mewakili data pengaturan halaman yang terdapat dalam format file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Mendapatkan induk dari objek View. Hanya-baca [`Project`](../project/). |
| [RepeatDetailsHeaderOnAllRows](../../aspose.tasks/usageview/repeatdetailsheaderonallrows/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah mengulangi header detail pada semua baris penugasan atau tidak. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Mendapatkan tipe layar untuk tampilan tunggal. Hanya-baca [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah Microsoft Project menampilkan nama tampilan tunggal di daftar drop-down View atau Other Views pada Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Mendapatkan atau mengatur tabel dari tampilan tunggal. |
| [TimescaleSizePercentage](../../aspose.tasks/usageview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/usageview/toptimescaletier/) { get; set; } | Mendapatkan atau mengatur pengaturan tingkat timescale atas tampilan. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

Menampilkan cara merender tampilan penggunaan tugas dengan detail.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// dapatkan tampilan
UsageView view = (TaskUsageView)project.DefaultView;

// kolom header detail tidak akan ditampilkan
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// tampilkan kolom header detail
view.DisplayDetailsHeaderColumn = true;

// ulangi header detail pada semua baris penugasan
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Lihat Juga

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



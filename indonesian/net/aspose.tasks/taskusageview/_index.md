---
title: "Kelas TaskUsageView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TaskUsageView. Mewakili tampilan penggunaan tugas dalam sebuah proyek"
type: docs
weight: 2480
url: /id/net/aspose.tasks/taskusageview/
---
## TaskUsageView class

Mewakili tampilan penggunaan tugas dalam proyek.

```csharp
public class TaskUsageView : UsageView
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AlignDetailsData](../../aspose.tasks/usageview/aligndetailsdata/) { get; set; } | Mendapatkan atau mengatur perataan data detail. |
| [BottomTimescaleTier](../../aspose.tasks/usageview/bottomtimescaletier/) { get; set; } | Mendapatkan atau mengatur pengaturan tingkat timescale bawah tampilan. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [DisplayDetailsHeaderColumn](../../aspose.tasks/usageview/displaydetailsheadercolumn/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan kolom header detail dalam tampilan atau tidak. |
| [DisplayShortDetailHeaderNames](../../aspose.tasks/usageview/displayshortdetailheadernames/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menampilkan nama header detail singkat atau tidak. |
| [FieldCollection](../../aspose.tasks/taskusageview/fieldcollection/) { get; } | Mendapatkan objek [`TaskUsageViewFieldCollection`](../taskusageviewfieldcollection/) dari TaskUsageView ini. |
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

Menunjukkan cara merender tampilan penggunaan tugas dengan pengaturan skala waktu yang didefinisikan dalam pengaturan tampilan.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Definisikan SaveOptions dan tentukan bahwa pengaturan skala waktu TaskUsageView harus digunakan.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

Menampilkan cara merender tampilan penggunaan tugas dengan pengaturan skala waktu yang telah ditentukan.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

// Definisikan SaveOptions dan tentukan pengaturan TimeScale yang telah ditentukan 'Days'.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Days,

    // Atur format Presentasi menjadi TaskUsage
    PresentationFormat = PresentationFormat.TaskUsage
};

var outputProject = "TaskUsageView_result_days_out.pdf";
project.Save(OutDir + outputProject, options);

// Atur pengaturan Timescale menjadi ThirdsOfMonths
options.Timescale = Timescale.ThirdsOfMonths;

outputProject = "TaskUsageView_result_thirdsOfMonths_out.pdf";
project.Save(OutDir + outputProject, options);

// Atur pengaturan Timescale menjadi Months
options.Timescale = Timescale.Months;

outputProject = "TaskUsageView_result_months_out.pdf";
project.Save(OutDir + outputProject, options);
```

### Lihat Juga

* class [UsageView](../usageview/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



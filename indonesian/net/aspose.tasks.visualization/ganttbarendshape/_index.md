---
title: "Enum GanttBarEndShape"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.GanttBarEndShape enum. Mewakili bentuk akhir pada batang dan titik kemajuan dalam garis kemajuan"
type: docs
weight: 3030
url: /id/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Mewakili bentuk akhir pada bar dan titik kemajuan dalam garis kemajuan.

```csharp
public enum GanttBarEndShape
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| ArrowDown | `14` | Menunjukkan panah mengarah ke bawah pada bentuk akhir batang Gantt. |
| ArrowUp | `8` | Menunjukkan panah mengarah ke atas pada bentuk akhir batang Gantt. |
| CaretDownTop | `9` | Menunjukkan Caret mengarah ke bawah pada setengah atas batang bentuk akhir batang Gantt. |
| CaretUpBottom | `10` | Menunjukkan Caret mengarah ke atas pada setengah bawah batang bentuk akhir batang Gantt. |
| Circle | `19` | Menunjukkan lingkaran pada bentuk akhir batang Gantt. |
| CircleArrowDown | `18` | Menunjukkan panah berlingkar mengarah ke bawah pada bentuk akhir batang Gantt. |
| CircleArrowUp | `17` | Menunjukkan panah berlingkar mengarah ke atas pada bentuk akhir batang Gantt. |
| CircleDiamond | `13` | Menunjukkan berlian berlingkar pada bentuk akhir batang Gantt. |
| CircleTriangleDown | `16` | Menunjukkan segitiga berlingkar mengarah ke bawah pada bentuk akhir batang Gantt. |
| CircleTriangleUp | `15` | Menunjukkan segitiga berlingkar mengarah ke atas pada bentuk akhir batang Gantt. |
| Diamond | `3` | Menunjukkan berlian pada bentuk akhir batang Gantt. |
| HouseDown | `2` | Menunjukkan rumah terbalik pada bentuk akhir batang Gantt. |
| HouseUp | `1` | Menunjukkan rumah pada bentuk akhir batang Gantt. |
| LeftBracket | `21` | Menunjukkan kurung kiri pada bentuk akhir batang Gantt. |
| LeftFade | `23` | Menunjukkan fade kiri pada bentuk akhir batang Gantt. |
| LineShape | `11` | Menunjukkan garis pada bentuk akhir batang Gantt. |
| NoBarEndShape | `0` | Menunjukkan tidak ada pada bentuk akhir batang Gantt. |
| RightBracket | `22` | Menunjukkan kurung kanan pada bentuk akhir batang Gantt. |
| RightFade | `24` | Menunjukkan fade kanan pada bentuk akhir batang Gantt. |
| Square | `12` | Menunjukkan persegi pada bentuk akhir batang Gantt. |
| Star | `20` | Menunjukkan bintang pada bentuk akhir batang Gantt. |
| TriangleDown | `5` | Menunjukkan segitiga mengarah ke bawah pada bentuk akhir batang Gantt. |
| TriangleLeft | `7` | Menunjukkan bentuk akhir bar Gantt segitiga mengarah ke kiri. |
| TriangleRight | `6` | Menunjukkan bentuk akhir bar Gantt segitiga mengarah ke kanan. |
| TriangleUp | `4` | Menunjukkan segitiga berlingkar mengarah ke atas pada bentuk akhir batang Gantt. |

## Contoh

Menampilkan cara mengatur gaya bar khusus pada tampilan proyek Gantt Chart.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Tambahkan gaya bar khusus ke koleksi bar khusus pada tampilan proyek
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

Menampilkan cara menggunakan gaya bar khusus pada tampilan Gantt Chart.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Gaya bar dapat bersifat khusus tugas (terletak di GanttChartView.CustomBarStyles)
// atau khusus kategori (terletak di GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Untuk tujuan demonstrasi, kami mengubah gaya untuk Tugas dengan ID Unik = 4
    // Di sini kami mengatur bidang (TaskName) untuk ditampilkan di sebelah kiri bar tugas.
    ganttBarStyle.LeftField = Field.TaskName;
    // Di sini kami mengatur konverter khusus untuk mengontrol teks apa yang harus ditampilkan di dalam bar tugas.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Untuk tujuan demonstrasi, kami mengubah gaya yang berlaku untuk tugas milestone.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



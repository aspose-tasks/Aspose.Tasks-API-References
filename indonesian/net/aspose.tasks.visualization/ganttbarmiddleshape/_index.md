---
title: "Enum GanttBarMiddleShape"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Menentukan bentuk tengah dari sebuah batang"
type: docs
weight: 3050
url: /id/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Menentukan bentuk tengah sebuah bar.

```csharp
public enum GanttBarMiddleShape
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| LineBottom | `7` | Menunjukkan bentuk garis yang diratakan ke bawah. |
| LineMiddle | `6` | Menunjukkan bentuk garis yang diratakan ke tengah. |
| LineTop | `5` | Menunjukkan bentuk garis yang diratakan ke atas. |
| None | `0` | Menunjukkan bentuk kosong. |
| RectangleBar | `1` | Menunjukkan bentuk batang persegi panjang dengan tinggi penuh. |
| RectangleBottom | `4` | Menunjukkan bentuk batang persegi panjang setengah tinggi yang diratakan ke bawah. |
| RectangleMiddle | `3` | Menunjukkan bentuk batang persegi panjang setinggi 1/3 yang diratakan ke tengah. |
| RectangleTop | `2` | Menunjukkan bentuk bar persegi panjang setengah tinggi yang diratakan ke atas. |

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



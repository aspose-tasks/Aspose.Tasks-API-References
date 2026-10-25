---
title: "GanttBarStyle.InsideBarTextConverter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti GanttBarStyle. Mendapatkan atau mengatur konverter yang didefinisikan pengguna untuk mendapatkan teks yang akan dirender di dalam bar tugas. Menimpa nilai properti InsideField"
type: docs
weight: 80
url: /id/net/aspose.tasks.visualization/ganttbarstyle/insidebartextconverter/
---
## GanttBarStyle.InsideBarTextConverter property

Mendapatkan atau mengatur konverter yang didefinisikan pengguna untuk mendapatkan teks yang akan dirender di dalam bar tugas. Menimpa nilai properti [`InsideField`](../insidefield/).

```csharp
public TaskBarTextConverter InsideBarTextConverter { get; set; }
```

## Catatan

Tidak disimpan ke format MPP.

## Contoh

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

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)



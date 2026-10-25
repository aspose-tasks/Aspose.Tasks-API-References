---
title: "TimelineView.TimelineView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor TimelineView. Menginisialisasi instance baru dari kelas TimelineView"
type: docs
weight: 10
url: /id/net/aspose.tasks/timelineview/timelineview/
---
## TimelineView constructor

Menginisialisasi instance baru dari kelas [`TimelineView`](../).

```csharp
public TimelineView()
```

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

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)



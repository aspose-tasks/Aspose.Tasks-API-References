---
title: "ProjectView.GetDefaultGanttChartView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectView. Menyertakan kolom tugas id, indikator, nama, durasi, mulai, dan selesai"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/projectview/getdefaultganttchartview/
---
## ProjectView.GetDefaultGanttChartView method

Menyertakan kolom id, indikator, nama, durasi, mulai, dan selesai tugas.

```csharp
public static ProjectView GetDefaultGanttChartView()
```

### Nilai Kembali

sebuah tampilan yang berisi daftar [`GanttChartColumn`](../../ganttchartcolumn/).

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan diagram Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultGanttChartView()
};

project.Save(OutDir + "WorkWithProjectView_GanttChartView_out.pdf", options);
```

### Lihat Juga

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



---
title: "ProjectView.GetDefaultTaskSheetView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectView. Menyertakan kolom tugas id, indikator, nama, durasi, mulai, selesai, pendahulu, dan nama sumber daya"
type: docs
weight: 60
url: /id/net/aspose.tasks.visualization/projectview/getdefaulttasksheetview/
---
## ProjectView.GetDefaultTaskSheetView method

Menyertakan id, indikator, nama, durasi, mulai, selesai, pendahulu, dan kolom tugas nama sumber daya.

```csharp
public static ProjectView GetDefaultTaskSheetView()
```

### Nilai Kembali

sebuah tampilan yang berisi daftar [`GanttChartColumn`](../../ganttchartcolumn/).

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan lembar tugas.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultTaskSheetView()
};

project.Save(OutDir + "WorkWithProjectView_TaskSheetView_out.pdf", options);
```

### Lihat Juga

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



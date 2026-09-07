---
title: "Class ProjectView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.ProjectView class. Kelas tampilan proyek"
type: docs
weight: 3300
url: /id/net/aspose.tasks.visualization/projectview/
---
## ProjectView class

Kelas tampilan proyek

```csharp
public class ProjectView
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ProjectView](projectview/)(IEnumerable&lt;ViewColumn&gt;) | Menginisialisasi sebuah instance baru dari kelas `ProjectView`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Columns](../../aspose.tasks.visualization/projectview/columns/) { get; } | Mendapatkan kolom tampilan proyek. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [GetDefaultAssignmentView](../../aspose.tasks.visualization/projectview/getdefaultassignmentview/)() | Menyertakan kolom Uid, nama tugas, nama sumber daya, pekerjaan, dan durasi penugasan. |
| static [GetDefaultGanttChartView](../../aspose.tasks.visualization/projectview/getdefaultganttchartview/)() | Menyertakan kolom id, indikator, nama, durasi, mulai, dan selesai tugas. |
| static [GetDefaultResourceSheetView](../../aspose.tasks.visualization/projectview/getdefaultresourcesheetview/)() | Menyertakan kolom Uid, nama sumber daya, tipe, label material, inisial, grup, unit maksimum, tarif standar, tarif lembur, biaya per penggunaan, akrual pada, kalender dasar, dan kode sumber daya. |
| static [GetDefaultResourceUsageView](../../aspose.tasks.visualization/projectview/getdefaultresourceusageview/)() | Menyertakan Uid, nama, mulai, selesai, dan kolom sumber daya kerja. |
| static [GetDefaultTaskSheetView](../../aspose.tasks.visualization/projectview/getdefaulttasksheetview/)() | Menyertakan id, indikator, nama, durasi, mulai, selesai, pendahulu, dan kolom tugas nama sumber daya. |

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan penugasan.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultAssignmentView()
};

project.Save(OutDir + "WorkWithProjectView_AssignmentView_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



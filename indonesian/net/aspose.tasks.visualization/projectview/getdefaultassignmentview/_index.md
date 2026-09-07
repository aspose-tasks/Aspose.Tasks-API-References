---
title: "ProjectView.GetDefaultAssignmentView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectView. Menyertakan kolom penugasan Uid, nama tugas, nama sumber daya, kerja, dan durasi"
type: docs
weight: 20
url: /id/net/aspose.tasks.visualization/projectview/getdefaultassignmentview/
---
## ProjectView.GetDefaultAssignmentView method

Menyertakan kolom Uid, nama tugas, nama sumber daya, pekerjaan, dan durasi penugasan.

```csharp
public static ProjectView GetDefaultAssignmentView()
```

### Nilai Kembali

sebuah tampilan yang berisi daftar [`AssignmentViewColumn`](../../assignmentviewcolumn/).

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

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



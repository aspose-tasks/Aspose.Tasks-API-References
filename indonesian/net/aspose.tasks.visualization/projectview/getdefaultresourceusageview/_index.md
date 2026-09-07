---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectView. Menyertakan kolom sumber daya uid, nama, mulai, selesai, dan kerja"
type: docs
weight: 50
url: /id/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Menyertakan Uid, nama, mulai, selesai, dan kolom sumber daya kerja.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Nilai Kembali

sebuah tampilan yang berisi daftar [`ResourceViewColumn`](../../resourceviewcolumn/).

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan penggunaan sumber daya.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### Lihat Juga

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ProjectView. Menyertakan kolom sumber daya Uid, nama, tipe, material, label, inisial, grup, unit maksimum, tarif standar, tarif lembur, biaya per penggunaan, akrual pada kalender dasar, dan kode"
type: docs
weight: 40
url: /id/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Menyertakan kolom Uid, nama sumber daya, tipe, label material, inisial, grup, unit maksimum, tarif standar, tarif lembur, biaya per penggunaan, akrual pada, kalender dasar, dan kode sumber daya.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Nilai Kembali

sebuah tampilan yang berisi daftar [`ResourceViewColumn`](../../resourceviewcolumn/).

## Contoh

Menampilkan cara menyimpan proyek dengan tampilan lembar sumber daya.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### Lihat Juga

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)



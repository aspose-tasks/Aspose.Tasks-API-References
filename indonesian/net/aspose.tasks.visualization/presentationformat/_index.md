---
title: "Enum PresentationFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Visualization.PresentationFormat enum. Enumerasi untuk format presentasi."
type: docs
weight: 3270
url: /id/net/aspose.tasks.visualization/presentationformat/
---
## PresentationFormat enumeration

Enumerasi untuk format presentasi.

```csharp
public enum PresentationFormat
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| GanttChart | `0` | Format presentasi Gantt Chart. |
| TaskUsage | `1` | Format presentasi penggunaan tugas. |
| ResourceUsage | `2` | Format presentasi penggunaan sumber daya. |
| ResourceSheet | `3` | Format presentasi lembar sumber daya. |
| TaskSheet | `4` | Format presentasi lembar tugas. |

## Contoh

Menampilkan cara merender tampilan lembar sumber daya.

```csharp
var project = new Project(DataDir + "ResourceSheetView.mpp");

SaveOptions options = new PdfSaveOptions();

// Atur Format Presentasi ke Lembar Sumber Daya
options.PresentationFormat = PresentationFormat.ResourceSheet;
project.Save(OutDir + "ResourceSheetView_out.pdf", options);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Kelas ApsLayoutBuilderOutOfMemoryException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.ApsLayoutBuilderOutOfMemoryException. Mewakili pengecualian yang terjadi ketika memori tidak cukup untuk melanjutkan pembuatan tata letak gambar"
type: docs
weight: 20
url: /id/net/aspose.tasks/apslayoutbuilderoutofmemoryexception/
---
## ApsLayoutBuilderOutOfMemoryException class

Mewakili pengecualian yang terjadi ketika memori tidak cukup untuk melanjutkan pembuatan tata letak gambar.

```csharp
public class ApsLayoutBuilderOutOfMemoryException : Exception
```

## Contoh

Menampilkan cara menyimpan proyek sebagai gambar dan menangkap pengecualian.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    var ganttChart = (GanttChartView)project.Views.ToList()[0];

    ganttChart.MiddleTimescaleTier.Unit = TimescaleUnit.Hours;
    ganttChart.BottomTimescaleTier.Unit = TimescaleUnit.Minutes;
    ganttChart.BottomTimescaleTier.Count = 1;

    var options = new ImageSaveOptions(SaveFileFormat.Png);
    options.Timescale = Timescale.DefinedInView;

    project.Save(OutDir + "SaveToStreamWithOptionsAndCatchException_out.mpp", options);
}
catch (ApsLayoutBuilderOutOfMemoryException ex)
{
    Console.WriteLine(ex.Message);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



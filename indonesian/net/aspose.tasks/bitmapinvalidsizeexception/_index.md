---
title: "Class BitmapInvalidSizeException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.BitmapInvalidSizeException class. Mewakili pengecualian yang terjadi ketika tidak cukup memori untuk membuat instance bitmap."
type: docs
weight: 140
url: /id/net/aspose.tasks/bitmapinvalidsizeexception/
---
## BitmapInvalidSizeException class

Mewakili pengecualian yang terjadi ketika tidak cukup memori untuk membuat instance bitmap.

```csharp
public class BitmapInvalidSizeException : Exception
```

## Contoh

Menampilkan cara menyimpan proyek sebagai gambar dan menangkap pengecualian ukuran tidak valid.

```csharp
try
{
    var project = new Project(DataDir + "Blank2010.mpp");

    GanttChartView view = (GanttChartView) project.Views.ToList()[0];
    var options = new ImageSaveOptions(SaveFileFormat.Png)
    {
        Timescale = Timescale.DefinedInView
    };

    view.MiddleTimescaleTier.Unit = TimescaleUnit.Minutes;
    view.MiddleTimescaleTier.Count = 1;

    project.Save(OutDir + "SaveToStreamAndCatchException_out.mpp", options);
}
catch (BitmapInvalidSizeException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



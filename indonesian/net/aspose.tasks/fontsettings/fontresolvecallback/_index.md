---
title: "FontSettings.FontResolveCallback"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti FontSettings. Mendapatkan atau menetapkan callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan"
type: docs
weight: 30
url: /id/net/aspose.tasks/fontsettings/fontresolvecallback/
---
## FontSettings.FontResolveCallback property

Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan font yang diresolusikan.

```csharp
public FontResolveCallbackDelegate FontResolveCallback { get; set; }
```

## Contoh

Menampilkan cara mengatur callback penyelesaian font khusus untuk mengeksekusi kode yang didefinisikan pengguna guna menetapkan font cadangan atau menggantikan font tertentu.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
};

options.FontSettings.FontResolveCallback = delegate(FontResolveEventArgs args)
{
    if (args.RequestedFontName != args.ResolvedFontName)
    {
        // Sepertinya font yang tepat tidak dapat ditemukan dan font cadangan telah ditetapkan.
        // Kita dapat mengganti font cadangan.
        args.ResolvedFontName = "Arial";
    }

    // Atau cukup menggantikan font tertentu:
    if (args.RequestedFontName == "Comic Sans MS")
    {
        args.ResolvedFontName = "Arial";
    }
};

project.Save(OutDir + "EstimatedMilestoneTasks_out3.pdf", options);
```

### Lihat Juga

* delegate [FontResolveCallbackDelegate](../../fontresolvecallbackdelegate/)
* class [FontSettings](../)
* namespace [Aspose.Tasks](../../fontsettings/)
* assembly [Aspose.Tasks](../../../)



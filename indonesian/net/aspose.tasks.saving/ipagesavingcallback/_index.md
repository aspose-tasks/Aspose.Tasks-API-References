---
title: "Antarmuka IPageSavingCallback"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Saving.IPageSavingCallback interface. Mewakili callback yang dipanggil ketika setiap halaman dalam dokumen multi halaman disimpan ke aliran terpisah."
type: docs
weight: 2020
url: /id/net/aspose.tasks.saving/ipagesavingcallback/
---
## IPageSavingCallback interface

Mewakili callback yang dipanggil ketika setiap halaman dalam dokumen multipage disimpan ke aliran terpisah.

```csharp
public interface IPageSavingCallback
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| [OnFinish](../../aspose.tasks.saving/ipagesavingcallback/onfinish/)() | Metode yang akan dipanggil ketika semua halaman telah ditulis. |
| [PageSaving](../../aspose.tasks.saving/ipagesavingcallback/pagesaving/)(PageSavingArgs) | Metode yang dipanggil ketika sebuah halaman disimpan ke aliran. |

## Contoh

Menampilkan cara menyimpan dokumen multi halaman ke aliran yang disediakan pengguna menggunakan callback penyimpanan halaman.

```csharp
[Test] 
public void UsePageSavingCallbackToSavePageToSeparateStreams()
{
    var project = new Project(DataDir + "Homemoveplan.mpp");

    var imageSaveOptions = new ImageSaveOptions(SaveFileFormat.Png);

    var callback = new CustomPageSavingCallback();
    imageSaveOptions.PageSavingCallback = callback;
    imageSaveOptions.RenderToSinglePage = false;
    project.Save(Stream.Null, imageSaveOptions);

    foreach (var streams in callback.PageStreams)
    {
        // proses setiap aliran halaman
    }
}

private sealed class CustomPageSavingCallback : IPageSavingCallback
{
    public List<MemoryStream> PageStreams { get; } = new List<MemoryStream>();

    public void PageSaving(PageSavingArgs args)
    {
        var memoryStream = new MemoryStream();
        args.Stream = memoryStream;
        args.KeepStreamOpen = false;
        this.PageStreams.Add(memoryStream);
    }

    public void OnFinish()
    {
    }
}
```

### Lihat Juga

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)



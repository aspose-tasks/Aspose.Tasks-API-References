---
title: "IPageSavingCallback.OnFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode IPageSavingCallback. Metode yang akan dipanggil ketika semua halaman telah ditulis"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/ipagesavingcallback/onfinish/
---
## IPageSavingCallback.OnFinish method

Metode yang akan dipanggil ketika semua halaman telah ditulis.

```csharp
public void OnFinish()
```

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

* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)



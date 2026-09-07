---
title: "IPageSavingCallback.PageSaving"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode IPageSavingCallback. Metode yang akan dipanggil ketika sebuah halaman disimpan ke aliran"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/ipagesavingcallback/pagesaving/
---
## IPageSavingCallback.PageSaving method

Metode yang dipanggil ketika sebuah halaman disimpan ke aliran.

```csharp
public void PageSaving(PageSavingArgs args)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| args | PageSavingArgs | Argumen penyimpanan halaman. |

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

* class [PageSavingArgs](../../pagesavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Tasks.Saving](../../ipagesavingcallback/)
* assembly [Aspose.Tasks](../../../)



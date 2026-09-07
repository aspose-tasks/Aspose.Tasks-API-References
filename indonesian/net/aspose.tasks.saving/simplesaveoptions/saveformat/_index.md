---
title: "SimpleSaveOptions.SaveFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SimpleSaveOptions. Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan"
type: docs
weight: 10
url: /id/net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan.

```csharp
public SaveFileFormat SaveFormat { get; }
```

## Contoh

Menampilkan cara menggunakan filter tugas khusus saat menyimpan file MS Project.

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // atur filter tugas untuk melewatkan tugas 'Task5' dan 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // mari periksa format penyimpanan
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // simpan proyek sebagai gambar
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Contoh filter tugas khusus yang dapat digunakan saat menyimpan file MS Project (misalnya) dalam format PDF.
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### Lihat Juga

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)



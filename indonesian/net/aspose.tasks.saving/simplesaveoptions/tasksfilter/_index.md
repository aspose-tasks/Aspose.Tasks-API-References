---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SimpleSaveOptions. Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang ditampilkan pada Lembar Tugas Gantt dan diagram Penggunaan Tugas"
type: docs
weight: 30
url: /id/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Catatan

Jika nilai tidak ditentukan, filter default akan digunakan yang menghapus tugas yang tidak terlihat -- yaitu tugas turunan dari tugas yang dikompres.

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

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)



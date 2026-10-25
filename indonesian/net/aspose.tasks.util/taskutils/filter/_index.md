---
title: "TaskUtils.Filter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskUtils. Membuat pohon baru tugas yang memenuhi kondisi"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Membangun pohon tugas baru yang memenuhi kondisi.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | Tugas | Akar pohon. |
| cond | ICondition`1 | Kondisi yang diterapkan. |

### Nilai Kembali

Akar pohon baru.

## Contoh

Menampilkan cara bekerja dengan sebuah kondisi.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // membuat pohon baru tugas yang memenuhi kondisi 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // mengumpulkan tugas dari sebuah pohon
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // mengiterasi daftar sederhana tugas 
    // yang durasinya lebih besar atau sama dengan 2 hari kerja
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Mengembalikan true jika objek yang ditentukan memenuhi kondisi.
    /// </summary>
    /// <param name=\"el\">Objek yang akan diperiksa.</param>
    /// <returns>True jika objek memenuhi kondisi.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)



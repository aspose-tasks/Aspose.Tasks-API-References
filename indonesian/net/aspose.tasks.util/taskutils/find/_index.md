---
title: "TaskUtils.Find"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode TaskUtils. Menemukan tugas yang memenuhi kondisi dalam pohon tugas."
type: docs
weight: 30
url: /id/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Menemukan tugas yang memenuhi kondisi dalam pohon tugas.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | Tugas | Akar pohon. |
| cond | ICondition`1 | Kondisi yang diterapkan. |

### Nilai Kembali

Task jika ditemukan, jika tidak null.

## Contoh

Menampilkan cara menggunakan &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; metode.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // membuat pohon baru tugas yang memenuhi kondisi 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Mengembalikan true jika objek yang ditentukan memenuhi kondisi.
    /// </summary>
    /// <param name=\"el\">Objek yang akan diperiksa.</param>
    /// <returns>True jika objek memenuhi kondisi.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)



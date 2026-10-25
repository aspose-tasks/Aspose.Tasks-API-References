---
title: "RemoveTask.PostAlg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode RemoveTask. Tidak melakukan apa-apa"
type: docs
weight: 30
url: /id/net/aspose.tasks.util/removetask/postalg/
---
## RemoveTask.PostAlg method

Tidak melakukan apa pun.

```csharp
public void PostAlg(Task el, int level)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | Tugas | Objek untuk diproses. |
| tingkat | Int32 | Level node pohon. |

## Contoh

Menampilkan cara menggunakan algoritma berbasis pohon &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt;.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // gunakan algoritma berbasis pohon untuk menghapus task1 dari pohon
    var algorithm = new RemoveTask(task1);

    // terapkan algoritma pada pohon tugas
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // periksa hasilnya
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)



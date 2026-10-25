---
title: "Kelas RemoveTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.RemoveTask. Menghapus tugas yang ditentukan dari pohon tugas."
type: docs
weight: 2760
url: /id/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Menghapus tugas yang ditentukan dari pohon tugas.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Menginisialisasi instance baru dari kelas `RemoveTask`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Tidak melakukan apa pun. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Tidak melakukan apa pun. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Menghapus tugas dari tugas induk yang ditentukan. |

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

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



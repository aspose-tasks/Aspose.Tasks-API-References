---
title: "Task.ToString"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengembalikan representasi string pendek dari sebuah tugas. Detail tepat dari representasi tidak ditentukan dan dapat berubah"
type: docs
weight: 1420
url: /id/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Mengembalikan representasi string singkat dari sebuah tugas. Detail tepat dari representasi tersebut tidak ditentukan dan dapat berubah.

```csharp
public override string ToString()
```

### Nilai Kembali

string pendek yang mewakili objek tugas.

## Contoh

Menampilkan cara mengurutkan tugas berdasarkan nama.

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



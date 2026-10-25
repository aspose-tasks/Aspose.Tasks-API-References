---
title: "AndAllCondition1.Check"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode AndAllCondition. Mengembalikan true jika objek yang ditentukan memenuhi kondisi"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

Mengembalikan true jika objek yang ditentukan memenuhi kondisi.

```csharp
public bool Check(T el)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang akan diperiksa. |

### Nilai Kembali

Benar jika objek memenuhi kondisi.

## Contoh

Menampilkan cara menggunakan kondisi &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // mengumpulkan semua tugas proyek
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // buat kondisi filter yang menyaring tugas yang tidak null
                             new NotNullCondition(),

                             // buat kondisi filter yang menyaring tugas ringkasan
                             new SummaryCondition()
                         };

    // dan menggabungkannya dengan menerapkan kondisi <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // terapkan kondisi pada tugas yang dikumpulkan
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // bekerja dengan properti lain...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### Lihat Juga

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)



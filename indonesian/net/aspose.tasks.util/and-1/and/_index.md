---
title: "And1.And"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor And. Menginisialisasi sebuah instance baru dari kelas And"
type: docs
weight: 10
url: /id/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

Menginisialisasi sebuah instance baru dari kelas [`And`](../).

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| cond1 | ICondition`1 | Kondisi pertama. |
| cond2 | ICondition`1 | Kondisi kedua. |

## Contoh

Menampilkan cara menggunakan kondisi &lt;see cref="Aspose.Tasks.Util.And`1" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // mengumpulkan semua tugas proyek
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // buat kondisi filter yang menyaring tugas ringkasan
    var condition1 = new SummaryCondition();

    // buat kondisi filter yang menyaring tugas yang tidak null
    var condition2 = new NotNullCondition();

    // dan gabungkan mereka dengan menerapkan kondisi <see cref="Aspose.Tasks.Util.And`1" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // terapkan kondisi pada tugas yang dikumpulkan
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)



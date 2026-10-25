---
title: "Not1.Not"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor Not. Menginisialisasi instance baru dari kelas Not."
type: docs
weight: 10
url: /id/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

Menginisialisasi instance baru dari kelas [`Not`](../).

```csharp
public Not(ICondition<T> condition)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| kondisi | ICondition`1 | Kondisi yang ditentukan. |

## Contoh

Menampilkan cara menggunakan kondisi &lt;see cref="Aspose.Tasks.Util.Not`1" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // mengumpulkan semua tugas proyek
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // buat kondisi filter
    var filter = new NullCondition();

    // dan balikkan dengan menerapkan kondisi <see cref="Aspose.Tasks.Util.Not`1" />
    var condition = new Not<Task>(filter);

    // terapkan kondisi pada tugas yang dikumpulkan
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Lihat Juga

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)



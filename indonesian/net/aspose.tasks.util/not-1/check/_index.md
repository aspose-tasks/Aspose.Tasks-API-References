---
title: "Not1.Check"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Not. Mengembalikan true jika objek yang ditentukan memenuhi kondisi."
type: docs
weight: 20
url: /id/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

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

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)



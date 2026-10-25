---
title: "Kelas NotT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.Not1T. Menerapkan NOT logika pada kondisi yang ditentukan"
type: docs
weight: 2750
url: /id/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Menerapkan NOT logika pada kondisi yang ditentukan.

```csharp
public class Not<T> : ICondition<T>
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan antarmuka metode. |

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Menginisialisasi instance baru dari kelas `Not`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



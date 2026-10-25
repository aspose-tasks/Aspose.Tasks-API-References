---
title: "Kelas AndAllConditionT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.AndAllCondition1T. Menerapkan logika AND pada semua kondisi. Misalnya cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /id/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Menerapkan AND logika pada semua kondisi. Misalnya: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan antarmuka metode. |

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Menginisialisasi instance baru dari kelas `AndAllCondition`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



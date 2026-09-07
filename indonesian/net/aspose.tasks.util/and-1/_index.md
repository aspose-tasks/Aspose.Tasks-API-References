---
title: "Kelas AndT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.And1T. Menerapkan AND logika pada kondisi yang ditentukan"
type: docs
weight: 2670
url: /id/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Menerapkan AND logika pada kondisi yang ditentukan.

```csharp
public class And<T> : ICondition<T>
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan antarmuka metode. |

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Menginisialisasi instance baru dari kelas `And`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



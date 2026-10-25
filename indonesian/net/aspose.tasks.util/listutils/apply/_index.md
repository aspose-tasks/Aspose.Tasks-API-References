---
title: "ListUtils.Apply"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ListUtils. Menerapkan algoritma untuk setiap elemen daftar mulai dari posisi yang ditentukan"
type: docs
weight: 10
url: /id/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

Terapkan algoritma untuk setiap elemen daftar mulai dari posisi yang ditentukan.

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan algoritma. |
| daftar | Daftar yang akan diproses. |
| algoritma | Algoritma yang diterapkan. |
| startIndex | Posisi elemen awal. |

## Contoh

Menunjukkan cara bekerja dengan metode Apply pada utilitas daftar.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### Lihat Juga

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



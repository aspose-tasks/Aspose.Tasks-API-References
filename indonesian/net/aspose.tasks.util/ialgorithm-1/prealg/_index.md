---
title: "IAlgorithm1.PreAlg"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode IAlgorithm. Dipanggil sebelum memproses sebuah objek."
type: docs
weight: 30
url: /id/net/aspose.tasks.util/ialgorithm-1/prealg/
---
## IAlgorithm&lt;T&gt;.PreAlg method

Dipanggil sebelum pemrosesan sebuah objek.

```csharp
public void PreAlg(T el, int index)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | T | Objek yang diproses. |
| index | Int32 | Indeks objek. |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)



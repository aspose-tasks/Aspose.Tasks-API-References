---
title: "Antarmuka IAlgorithmT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Antarmuka Aspose.Tasks.Util.IAlgorithm1T. Mewakili algoritma yang dapat diterapkan pada daftar objek T"
type: docs
weight: 2710
url: /id/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Mewakili algoritma yang dapat diterapkan pada daftar objek *T*.

```csharp
public interface IAlgorithm<in T>
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan antarmuka metode. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Memproses sebuah objek dalam daftar. Dipanggil setelah [`PreAlg`](./prealg/); |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Dipanggil setelah pemrosesan sebuah objek. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Dipanggil sebelum pemrosesan sebuah objek. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



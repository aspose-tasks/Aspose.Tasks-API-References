---
title: "ListUtils.Filter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ListUtils. Menyaring elemen daftar berdasarkan kondisi yang ditentukan"
type: docs
weight: 20
url: /id/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Filter elemen daftar berdasarkan kondisi yang ditentukan.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan filter. |
| daftar | Daftar yang akan diproses. |
| cond | Kondisi yang digunakan untuk menyaring daftar yang ditentukan. |

### Nilai Kembali

Daftar yang disaring.

## Contoh

Menampilkan cara bekerja dengan metode Filter pada utilitas daftar.

```csharp
public void WorkWithListUtilsFilter()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Filter(filters, new FilterByIndex(1));

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

public class FilterByIndex : ICondition<Filter>
{
    private readonly int index;

    public FilterByIndex(int index)
    {
        this.index = index;
    }

    /// <summary>
    /// Mengembalikan true jika objek yang ditentukan memenuhi kondisi.
    /// </summary>
    /// <param name=\"el\">Objek yang akan diperiksa.</param>
    /// <returns>True jika objek memenuhi kondisi.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Lihat Juga

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



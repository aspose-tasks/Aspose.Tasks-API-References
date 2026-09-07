---
title: "ICondition1.Check"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ICondition. Mengembalikan true jika objek yang ditentukan memenuhi kondisi"
type: docs
weight: 10
url: /id/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)



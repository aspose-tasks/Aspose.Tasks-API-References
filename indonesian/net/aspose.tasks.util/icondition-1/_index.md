---
title: "Antarmuka IConditionT"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Antarmuka Aspose.Tasks.Util.ICondition1T. Mewakili kondisi yang dapat digunakan oleh filter atau metode pencarian"
type: docs
weight: 2720
url: /id/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Mewakili kondisi yang dapat digunakan oleh filter atau metode pencarian.

```csharp
public interface ICondition<in T>
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan diterapkan antarmuka metode. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Mengembalikan true jika objek yang ditentukan memenuhi kondisi. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



---
title: "Kelas ListUtils"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Util.ListUtils. Kelas utilitas untuk pemrosesan daftar"
type: docs
weight: 2740
url: /id/net/aspose.tasks.util/listutils/
---
## ListUtils class

Kelas utilitas untuk pemrosesan daftar.

```csharp
public static class ListUtils
```

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Terapkan algoritma untuk setiap elemen daftar mulai dari posisi yang ditentukan. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Filter elemen daftar berdasarkan kondisi yang ditentukan. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Temukan kemunculan pertama dari elemen daftar yang memenuhi kondisi yang ditentukan. |

## Contoh

Menampilkan cara bekerja dengan metode Find pada utilitas daftar.

```csharp
public void WorkWithListUtilsFind()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> taskFilters = project.TaskFilters.ToList();

    Assert.AreEqual(3, taskFilters.Count, "Project.TaskFilters count");

    var filter = ListUtils.Find(taskFilters, new FilterByName("&All Tasks"));

    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Filter Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

public class FilterByName : ICondition<Filter>
{
    private readonly string name;

    public FilterByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Mengembalikan true jika objek yang ditentukan memenuhi kondisi.
    /// </summary>
    /// <param name=\"el\">Objek yang akan diperiksa.</param>
    /// <returns>True jika objek memenuhi kondisi.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Lihat Juga

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



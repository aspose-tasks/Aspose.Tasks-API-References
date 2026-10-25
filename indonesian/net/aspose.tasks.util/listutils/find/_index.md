---
title: "ListUtils.Find"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ListUtils. Menemukan kemunculan pertama dari elemen daftar yang memenuhi kondisi yang ditentukan"
type: docs
weight: 30
url: /id/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Temukan kemunculan pertama dari elemen daftar yang memenuhi kondisi yang ditentukan.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe objek yang akan dicari. |
| daftar | Daftar yang akan diproses. |
| cond | Kondisi yang digunakan untuk menemukan elemen dalam daftar yang ditentukan. |

### Nilai Kembali

Elemen daftar atau null.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



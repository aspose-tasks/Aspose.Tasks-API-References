---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ListUtils yöntemi. Belirtilen koşula göre liste öğelerini filtrele"
type: docs
weight: 20
url: /tr/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

Liste öğelerini belirtilen koşula göre filtrele.

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| Parametre | Açıklama |
| --- | --- |
| T | Filtre uygulanacak nesnenin türü. |
| liste | İşlenecek bir liste. |
| cond | Belirtilen listeyi filtrelemek için kullanılan koşul. |

### Dönüş Değeri

Filtrelenmiş liste.

## Örnekler

list util Filter yönteminin nasıl kullanılacağını gösterir.

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
    /// Belirtilen nesne koşulları karşılıyorsa true döndürür.
    /// </summary>
    /// <param name=\"el\">Kontrol edilecek nesne.</param>
    /// <returns>Nesne koşulları karşılıyorsa true döndürür.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### Ayrıca Bakınız

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



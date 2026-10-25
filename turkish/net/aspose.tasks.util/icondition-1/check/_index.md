---
title: "ICondition1.Check"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ICondition yöntemi. Belirtilen nesne koşulları sağlıyorsa true döndürür."
type: docs
weight: 10
url: /tr/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

Belirtilen nesne koşulları sağlarsa true döndürür.

```csharp
public bool Check(T el)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | T | Kontrol edilecek nesne. |

### Dönüş Değeri

Nesne koşulları sağlarsa doğru.

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)



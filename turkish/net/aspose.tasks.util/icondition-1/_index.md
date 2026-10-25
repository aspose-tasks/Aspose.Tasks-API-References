---
title: "Arayüz IConditionT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.ICondition1T arayüzü. Filtreler veya arama yöntemleri tarafından kullanılabilen bir koşulu temsil eder."
type: docs
weight: 2720
url: /tr/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

Filtreler veya arama yöntemleri tarafından kullanılabilecek bir koşulu temsil eder.

```csharp
public interface ICondition<in T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | Belirtilen nesne koşulları sağlarsa true döndürür. |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



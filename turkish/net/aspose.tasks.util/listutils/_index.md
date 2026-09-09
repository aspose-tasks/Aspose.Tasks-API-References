---
title: "Sınıf ListUtils"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.ListUtils sınıfı. Liste işleme için yardımcı sınıf"
type: docs
weight: 2740
url: /tr/net/aspose.tasks.util/listutils/
---
## ListUtils class

Liste işleme için yardımcı sınıf.

```csharp
public static class ListUtils
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | Belirtilen konumdan başlayarak her liste öğesi için algoritmayı uygula. |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Liste öğelerini belirtilen koşula göre filtrele. |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | Belirtilen koşulu sağlayan bir liste öğesinin ilk oluşumunu bul. |

## Örnekler

Liste yardımcı programının Find metoduyla nasıl çalışılacağını gösterir.

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
    /// Belirtilen nesne koşulları karşılıyorsa true döndürür.
    /// </summary>
    /// <param name=\"el\">Kontrol edilecek nesne.</param>
    /// <returns>Nesne koşulları karşılıyorsa true döndürür.</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



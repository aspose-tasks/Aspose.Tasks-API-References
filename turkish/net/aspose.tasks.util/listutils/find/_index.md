---
title: "ListUtils.Find"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ListUtils yöntemi. Belirtilen koşulu sağlayan bir liste öğesinin ilk oluşumunu bul"
type: docs
weight: 30
url: /tr/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

Belirtilen koşulu sağlayan bir liste öğesinin ilk oluşumunu bul.

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| Parametre | Açıklama |
| --- | --- |
| T | Bulunacak nesnenin türü. |
| liste | İşlenecek bir liste. |
| cond | Belirtilen listede bir öğeyi bulmak için kullanılan koşul. |

### Dönüş Değeri

Liste öğesi veya null.

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



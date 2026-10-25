---
title: "Arayüz IAlgorithmT"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Util.IAlgorithm1T arayüzü. T nesnelerinin bir listesine uygulanabilen bir algoritmayı temsil eder"
type: docs
weight: 2710
url: /tr/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

*T* nesnelerinin bir listesine uygulanabilen bir algoritmayı temsil eder.

```csharp
public interface IAlgorithm<in T>
```

| Parametre | Açıklama |
| --- | --- |
| T | Yöntem arayüzünün uygulanacağı nesnenin türü. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Listedeki bir nesneyi işler. [`PreAlg`](./prealg/) sonrası çağrılır; |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Bir nesnenin işlenmesinden sonra çağrılır. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Bir nesnenin işlenmesinden önce çağrılır. |

## Örnekler

Liste yardımcı Apply metodunun nasıl kullanılacağını gösterir.

```csharp
public void WorkWithListUtilsApply()
{
    var project = new Project(DataDir + "Project2003.mpp");
    List<Filter> filters = project.TaskFilters.ToList();

    Assert.AreEqual(3, filters.Count, "Project.TaskFilters count");

    ListUtils.Apply(filters, new RenameAlgorithm(), 0);

    foreach (var filter in filters)
    {
        Console.WriteLine("Name: " + filter.Name);
        Console.WriteLine("Filter Type: " + filter.FilterType);
        Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
        Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
        Console.WriteLine();
    }
}

private class RenameAlgorithm : IAlgorithm<Filter>
{
    private int current;

    public RenameAlgorithm()
    {
        this.current = 0;
    }

    public void PreAlg(Filter el, int index)
    {
        this.current++;
    }

    public void Alg(Filter el, int index)
    {
        el.Name = el.Name + " " + this.current;
    }

    public void PostAlg(Filter el, int index)
    {
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



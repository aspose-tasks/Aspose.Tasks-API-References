---
title: "इंटरफ़ेस IAlgorithmT"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.IAlgorithm1T इंटरफ़ेस। एक एल्गोरिदम का प्रतिनिधित्व करता है जिसे T वस्तुओं की सूची पर लागू किया जा सकता है"
type: docs
weight: 2710
url: /hi/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

*T* वस्तुओं की सूची पर लागू की जा सकने वाली एल्गोरिद्म का प्रतिनिधित्व करता है।

```csharp
public interface IAlgorithm<in T>
```

| पैरामीटर | विवरण |
| --- | --- |
| T | विधि इंटरफ़ेस लागू करने के लिए वस्तु का प्रकार। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | सूची में एक वस्तु को प्रोसेस करता है। [`PreAlg`](./prealg/) के बाद बुलाया जाता है; |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | वस्तु के प्रोसेसिंग के बाद बुलाया जाता है। |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | वस्तु के प्रोसेसिंग से पहले बुलाया जाता है। |

## उदाहरण

सूची उपयोगकर्ता Apply मेथड के साथ काम करने का तरीका दिखाता है।

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

### संबंधित देखें

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



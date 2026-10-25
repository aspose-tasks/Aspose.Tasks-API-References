---
title: "IAlgorithm1.Alg"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "IAlgorithm मेथड। सूची में एक ऑब्जेक्ट को प्रोसेस करता है। PreAlg के बाद कॉल किया जाता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/ialgorithm-1/alg/
---
## IAlgorithm&lt;T&gt;.Alg method

सूची में एक ऑब्जेक्ट को प्रोसेस करता है। [`PreAlg`](../prealg/) के बाद कॉल किया जाता है;

```csharp
public void Alg(T el, int index)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | प्रोसेस किया गया ऑब्जेक्ट। |
| इंडेक्स | Int32 | ऑब्जेक्ट का इंडेक्स। |

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

* interface [IAlgorithm&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../ialgorithm-1/)
* assembly [Aspose.Tasks](../../../)



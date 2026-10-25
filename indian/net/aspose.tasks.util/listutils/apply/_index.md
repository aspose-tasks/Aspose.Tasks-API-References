---
title: "ListUtils.Apply"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ListUtils मेथड। निर्दिष्ट स्थिति से शुरू होकर प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/listutils/apply/
---
## ListUtils.Apply&lt;T&gt; method

निर्दिष्ट स्थिति से शुरू करके प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें।

```csharp
public static void Apply<T>(IList<T> list, IAlgorithm<T> algorithm, int startIndex)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | एल्गोरिदम लागू करने वाले ऑब्जेक्ट का प्रकार। |
| सूची | प्रसंस्करण के लिए सूची। |
| एल्गोरिदम | लागू किया गया एल्गोरिदम। |
| startIndex | प्रारंभिक तत्व की स्थिति। |

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

* interface [IAlgorithm&lt;T&gt;](../../ialgorithm-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



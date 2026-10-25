---
title: "ListUtils.Filter"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ListUtils मेथड। निर्दिष्ट शर्त के आधार पर सूची तत्वों को फ़िल्टर करें"
type: docs
weight: 20
url: /hi/net/aspose.tasks.util/listutils/filter/
---
## ListUtils.Filter&lt;T&gt; method

निर्दिष्ट शर्त के आधार पर सूची तत्वों को फ़िल्टर करें।

```csharp
public static IList<T> Filter<T>(IList<T> list, ICondition<T> cond)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | फ़िल्टर लागू करने वाले ऑब्जेक्ट का प्रकार। |
| सूची | प्रसंस्करण के लिए एक सूची। |
| cond | निर्दिष्ट सूची को फ़िल्टर करने के लिए उपयोग की गई शर्त। |

### रिटर्न वैल्यू

फ़िल्टर की गई सूची।

## उदाहरण

दिखाता है कि सूची उपयोग फ़िल्टर मेथड के साथ कैसे काम किया जाए।

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
    /// निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है।
    /// </summary>
    /// <param name=\"el\">जाँचने वाली वस्तु।</param>
    /// <returns>यदि वस्तु शर्तों को पूरा करती है तो True।</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Index == this.index;
    }
}
```

### संबंधित देखें

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



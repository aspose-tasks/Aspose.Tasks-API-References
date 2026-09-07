---
title: "ICondition1.Check"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ICondition मेथड। यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है।"
type: docs
weight: 10
url: /hi/net/aspose.tasks.util/icondition-1/check/
---
## ICondition&lt;T&gt;.Check method

यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है।

```csharp
public bool Check(T el)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| el | T | जाँचने के लिए वस्तु। |

### रिटर्न वैल्यू

यदि वस्तु शर्तों को पूरा करती है तो सत्य।

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

* interface [ICondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../icondition-1/)
* assembly [Aspose.Tasks](../../../)



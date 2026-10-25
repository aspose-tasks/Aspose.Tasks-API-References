---
title: "इंटरफ़ेस IConditionT"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.ICondition1T इंटरफ़ेस। एक शर्त का प्रतिनिधित्व करता है जिसे फ़िल्टर या खोज विधियों द्वारा उपयोग किया जा सकता है"
type: docs
weight: 2720
url: /hi/net/aspose.tasks.util/icondition-1/
---
## ICondition&lt;T&gt; interface

फ़िल्टर या खोज विधियों द्वारा उपयोग की जा सकने वाली शर्त का प्रतिनिधित्व करता है।

```csharp
public interface ICondition<in T>
```

| पैरामीटर | विवरण |
| --- | --- |
| T | विधि इंटरफ़ेस लागू करने के लिए वस्तु का प्रकार। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Check](../../aspose.tasks.util/icondition-1/check/)(T) | यदि निर्दिष्ट ऑब्जेक्ट शर्तों को पूरा करता है तो true लौटाता है। |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



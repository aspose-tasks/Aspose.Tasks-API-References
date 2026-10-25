---
title: "ListUtils.Find"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ListUtils मेथड। निर्दिष्ट शर्त को पूरा करने वाले सूची तत्व की पहली उपस्थिति खोजें"
type: docs
weight: 30
url: /hi/net/aspose.tasks.util/listutils/find/
---
## ListUtils.Find&lt;T&gt; method

निर्दिष्ट शर्त को पूरा करने वाले सूची तत्व की पहली उपस्थिति खोजें।

```csharp
public static T Find<T>(IList<T> list, ICondition<T> cond)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | खोजने वाले ऑब्जेक्ट का प्रकार। |
| सूची | प्रसंस्करण के लिए एक सूची। |
| cond | निर्दिष्ट सूची में तत्व खोजने के लिए उपयोग की गई शर्त। |

### रिटर्न वैल्यू

सूची तत्व या null।

## उदाहरण

दिखाता है कि सूची उपयोगिता Find मेथड के साथ कैसे काम करें।

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
    /// निर्दिष्ट वस्तु शर्तों को पूरा करती है तो true लौटाता है।
    /// </summary>
    /// <param name=\"el\">जाँचने वाली वस्तु।</param>
    /// <returns>यदि वस्तु शर्तों को पूरा करती है तो True।</returns>
    /// <inheritdoc />
    public bool Check(Filter el)
    {
        return el.Name == this.name;
    }
}
```

### संबंधित देखें

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [ListUtils](../)
* namespace [Aspose.Tasks.Util](../../listutils/)
* assembly [Aspose.Tasks](../../../)



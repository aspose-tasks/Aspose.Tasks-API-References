---
title: "क्लास ListUtils"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Util.ListUtils क्लास। सूची प्रसंस्करण के लिए उपयोगी क्लास"
type: docs
weight: 2740
url: /hi/net/aspose.tasks.util/listutils/
---
## ListUtils class

सूची प्रसंस्करण के लिए उपयोगिता क्लास।

```csharp
public static class ListUtils
```

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [Apply&lt;T&gt;](../../aspose.tasks.util/listutils/apply/)(IList&lt;T&gt;, IAlgorithm&lt;T&gt;, int) | निर्दिष्ट स्थिति से शुरू करके प्रत्येक सूची तत्व पर एल्गोरिदम लागू करें। |
| static [Filter&lt;T&gt;](../../aspose.tasks.util/listutils/filter/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | निर्दिष्ट शर्त के आधार पर सूची तत्वों को फ़िल्टर करें। |
| static [Find&lt;T&gt;](../../aspose.tasks.util/listutils/find/)(IList&lt;T&gt;, ICondition&lt;T&gt;) | निर्दिष्ट शर्त को पूरा करने वाले सूची तत्व की पहली उपस्थिति खोजें। |

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

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)



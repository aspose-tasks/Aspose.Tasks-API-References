---
title: "क्लास FilterCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.FilterCollection क्लास। Filter ऑब्जेक्ट्स की एक सूची रखती है। ICollectionFilter इंटरफ़ेस को लागू करती है।"
type: docs
weight: 610
url: /hi/net/aspose.tasks/filtercollection/
---
## FilterCollection class

एक सूची रखता है [`Filter`](../filter/) ऑब्जेक्ट्स। ICollection&lt;Filter&gt; इंटरफ़ेस को इम्प्लीमेंट करता है।

```csharp
public class FilterCollection : ICollection<Filter>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | इस संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-रीड है या नहीं; अन्यथा, false। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | निर्दिष्ट आइटम को इस संग्रह में जोड़ता है। |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | इस संग्रह से सभी आइटम हटाता है। |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false। |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | निर्दिष्ट एरे सूचकांक से शुरू करके इस संग्रह के तत्वों को निर्दिष्ट एरे में कॉपी करता है। |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | इस संग्रह से विशिष्ट वस्तु की पहली घटना को हटाता है। |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | फ़िल्टर संग्रह को [`Filter`](../filter/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

फ़िल्टर संग्रहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// टास्क फ़िल्टरों पर इटरेट करें
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// रिसोर्स फ़िल्टरों पर इटरेट करें
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// अन्य प्रोजेक्ट के फ़िल्टर साफ़ करें
otherProject.TaskFilters.Clear();

// फ़िल्टरों को अन्य प्रोजेक्ट में कॉपी करें
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// कस्टम टास्क फ़िल्टर जोड़ें
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// सभी फ़िल्टर हटाएँ
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### संबंधित देखें

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



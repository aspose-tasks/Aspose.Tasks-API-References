---
title: "Filter.ShowInMenu"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter प्रॉपर्टी। एक मान प्राप्त या सेट करता है जो दर्शाता है कि प्रोजेक्ट व्यू टैब के रिबन में फ़िल्टर ड्रॉपडाउन सूची में फ़िल्टर नाम दिखाता है या नहीं"
type: docs
weight: 60
url: /hi/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

प्रोजेक्ट फ़िल्टर नाम को रिबन के व्यू टैब पर फ़िल्टर ड्रॉप-डाउन सूची में दिखाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool ShowInMenu { get; set; }
```

## उदाहरण

फ़िल्टर के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// संसाधन फ़िल्टर जांचें
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### संबंधित देखें

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)



---
title: "Filter.FilterType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Filter property. फ़िल्टर का प्रकार प्राप्त करता है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks/filter/filtertype/
---
## Filter.FilterType property

फ़िल्टर का प्रकार प्राप्त करता है।

```csharp
public ItemType FilterType { get; set; }
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

* enum [ItemType](../../itemtype/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)



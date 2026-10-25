---
title: "एन्यूम ItemType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.ItemType एन्यूम। किसी आइटम के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 920
url: /hi/net/aspose.tasks/itemtype/
---
## ItemType enumeration

किसी आइटम के प्रकार को निर्दिष्ट करता है।

```csharp
public enum ItemType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| TaskItem | `0` | टास्क आइटम। |
| ResourceItem | `1` | रिसोर्स आइटम। |
| OtherItem | `2` | अन्य आइटम। |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



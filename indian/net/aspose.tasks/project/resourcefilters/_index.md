---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। सभी रिसोर्स-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। ResourceFilters फ़िल्टर ऑब्जेक्ट्स का एक संग्रह है।"
type: docs
weight: 760
url: /hi/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

सभी रिसोर्स-आधारित फ़िल्टर परिभाषाएँ प्राप्त करता है। ResourceFilters [`Filter`](../../filter/) ऑब्जेक्ट्स का एक संग्रह है।

```csharp
public FilterCollection ResourceFilters { get; }
```

## उदाहरण

दिखाता है कि टास्क/रिसोर्स फ़िल्टर परिभाषाएँ कैसे पढ़ी जाएँ।

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// रिसोर्स फ़िल्टर तक पहुँचें
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### संबंधित देखें

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)



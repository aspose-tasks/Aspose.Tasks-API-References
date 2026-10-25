---
title: "FilterCollection.Contains"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "FilterCollection मेथड। यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है, अन्यथा false।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/filtercollection/contains/
---
## FilterCollection.Contains method

यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true लौटाता है; अन्यथा false।

```csharp
public bool Contains(Filter item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | Filter | खोजने के लिए निर्दिष्ट आइटम। |

### रिटर्न वैल्यू

यदि निर्दिष्ट आइटम इस संग्रह में पाया जाता है तो true; अन्यथा false।

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)



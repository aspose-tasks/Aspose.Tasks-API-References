---
title: "Group.MaintainHierarchy"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Group प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि समूह के भीतर सबटास्क के लिए सभी स्तरों के सारांश टास्क दिखाए जाएँ या नहीं"
type: docs
weight: 40
url: /hi/net/aspose.tasks/group/maintainhierarchy/
---
## Group.MaintainHierarchy property

समूह के भीतर सबटास्क के लिए सारांश टास्क के सभी स्तर दिखाने चाहिए या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है।

```csharp
public bool MaintainHierarchy { get; set; }
```

## उदाहरण

समूहों के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Uid: " + group.Uid);
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Is Task Group Maintain Hierarchy?: " + group.MaintainHierarchy);
Console.WriteLine("Is Task Group Show In Menu?: " + group.ShowInMenu);
Console.WriteLine("Is Task Group Show Summary?: " + group.ShowSummary);
Console.WriteLine("Is Task Group should groups Assignments instead of Tasks?: " + group.GroupAssignments);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);
Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");

foreach (var criterion in group.GroupCriteria)
{
    Console.WriteLine("Task Criterion Field: " + criterion.Field);
    Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
    Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
    Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

    Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
    Console.WriteLine("Font Size: " + criterion.Font.Size);
    Console.WriteLine("Font Style: " + criterion.Font.Style);
    Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
}
```

### संबंधित देखें

* class [Group](../)
* namespace [Aspose.Tasks](../../group/)
* assembly [Aspose.Tasks](../../../)



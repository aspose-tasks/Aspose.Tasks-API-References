---
title: "GroupCriterion.Pattern"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GroupCriterion प्रॉपर्टी। समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के सेल पैटर्न को प्राप्त करता है या सेट करता है।"
type: docs
weight: 90
url: /hi/net/aspose.tasks/groupcriterion/pattern/
---
## GroupCriterion.Pattern property

समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के लिए सेल के पैटर्न को प्राप्त करता है या सेट करता है।

```csharp
public BackgroundPattern Pattern { get; set; }
```

## उदाहरण

दिखाता है कि समूह मानदंड की गुणों को कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "ReadGroupDefinitionData.mpp");

Console.WriteLine("Task Groups Count: " + project.TaskGroups.Count);
var group = project.TaskGroups.ToList()[1];
Console.WriteLine("Task Group Name: " + group.Name);
Console.WriteLine("Task Group Criteria count: " + group.GroupCriteria.Count);

Console.WriteLine("\n************* Retrieving Task Group's Criterion information *************");
var criterion = group.GroupCriteria.ToList()[0];
Console.WriteLine("Task Criterion Field: " + criterion.Field);
Console.WriteLine("Task Criterion GroupOn: " + criterion.GroupOn);
Console.WriteLine("Task Criterion Cell Color: " + criterion.CellColor);
Console.WriteLine("Task Criterion Font Color: " + criterion.FontColor);
Console.WriteLine("Task Criterion Group Interval: " + criterion.GroupInterval);
Console.WriteLine("Task Criterion Start At: " + criterion.StartAt);

// मानदंड की पृष्ठभूमि पैटर्न पढ़ें।
Console.WriteLine("Task Criterion Pattern: " + criterion.Pattern);

Console.WriteLine("\n*********** Retrieving Criterion's Font Information ***********");
Console.WriteLine("Font Name: " + criterion.Font.FontFamily);
Console.WriteLine("Font Size: " + criterion.Font.Size);
Console.WriteLine("Font Style: " + criterion.Font.Style);
Console.WriteLine("Ascending/Descending: " + criterion.Ascending);
```

### संबंधित देखें

* enum [BackgroundPattern](../../backgroundpattern/)
* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)



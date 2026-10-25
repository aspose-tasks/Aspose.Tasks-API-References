---
title: "GroupCriterion.Ascending"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "GroupCriterion प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड को आरोही क्रम में सॉर्ट किया गया है या नहीं। यदि फ़ील्ड को अवरोही क्रम में सॉर्ट किया गया है तो यह फ़ॉल्स है।"
type: docs
weight: 20
url: /hi/net/aspose.tasks/groupcriterion/ascending/
---
## GroupCriterion.Ascending property

एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि समूह परिभाषा में मानदंड के रूप में उपयोग किया गया फ़ील्ड आरोही क्रम में सॉर्ट किया गया है या नहीं। यदि फ़ील्ड अवरोही क्रम में सॉर्ट किया गया है तो यह false होता है।

```csharp
public bool Ascending { get; set; }
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

* class [GroupCriterion](../)
* namespace [Aspose.Tasks](../../groupcriterion/)
* assembly [Aspose.Tasks](../../../)



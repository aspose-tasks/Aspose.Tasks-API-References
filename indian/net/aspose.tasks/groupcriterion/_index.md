---
title: "क्लास GroupCriterion"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.GroupCriterion क्लास। समूह परिभाषा में एक मानदंड का प्रतिनिधित्व करता है। GroupCriterion ऑब्जेक्ट GroupCriterionCollection संग्रह का सदस्य है।"
type: docs
weight: 790
url: /hi/net/aspose.tasks/groupcriterion/
---
## GroupCriterion class

समूह परिभाषा में एक मानदंड का प्रतिनिधित्व करता है। GroupCriterion ऑब्जेक्ट [`GroupCriterionCollection`](../groupcriterioncollection/) संग्रह का सदस्य है।

```csharp
public class GroupCriterion
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [GroupCriterion](groupcriterion/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Ascending](../../aspose.tasks/groupcriterion/ascending/) { get; set; } | एक मान प्राप्त करता है या सेट करता है जो दर्शाता है कि समूह परिभाषा में मानदंड के रूप में उपयोग किया गया फ़ील्ड आरोही क्रम में सॉर्ट किया गया है या नहीं। यदि फ़ील्ड अवरोही क्रम में सॉर्ट किया गया है तो यह false होता है। |
| [CellColor](../../aspose.tasks/groupcriterion/cellcolor/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के सेल बैकग्राउंड का रंग प्राप्त करता है या सेट करता है। |
| [Field](../../aspose.tasks/groupcriterion/field/) { get; set; } | समूहित किए जा रहे फ़ील्ड को प्राप्त करता है या सेट करता है। |
| [Font](../../aspose.tasks/groupcriterion/font/) { get; set; } | समूह परिभाषा में मानदंड के लिए फ़ॉन्ट प्राप्त करता है या सेट करता है। |
| [FontColor](../../aspose.tasks/groupcriterion/fontcolor/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के फ़ॉन्ट का रंग प्राप्त करता है या सेट करता है। |
| [GroupInterval](../../aspose.tasks/groupcriterion/groupinterval/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड का अंतराल प्राप्त करता है या सेट करता है। |
| [GroupOn](../../aspose.tasks/groupcriterion/groupon/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के समूह प्रकार को प्राप्त करता है या सेट करता है। |
| [Pattern](../../aspose.tasks/groupcriterion/pattern/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के लिए सेल के पैटर्न को प्राप्त करता है या सेट करता है। |
| [StartAt](../../aspose.tasks/groupcriterion/startat/) { get; set; } | समूह परिभाषा में मानदंड के रूप में उपयोग किए गए फ़ील्ड के अंतराल की शुरुआत को प्राप्त करता है या सेट करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| override [Equals](../../aspose.tasks/groupcriterion/equals/)(object) | यह संकेत देने वाला मान लौटाता है कि यह उदाहरण निर्दिष्ट ऑब्जेक्ट के बराबर है या नहीं। |
| override [GetHashCode](../../aspose.tasks/groupcriterion/gethashcode/)() | किसी विशेष प्रकार के लिए हैश फ़ंक्शन के रूप में कार्य करता है। |

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

प्रोजेक्ट में समूह जोड़ने का तरीका दर्शाता है।

```csharp
var p = new Project();

{
    var group = new Group();
    group.Name = "My new task group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.TaskDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 13F, FontStyles.Italic);
    criterion.GroupOn = GroupOn.DurationMinutes;
    criterion.StartAt = 5;
    criterion.GroupInterval = 3D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.TaskPercentComplete;
    criterion2.Font = new FontDescriptor("Bodoni MT", 17, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Pct199;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Green;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.TaskGroups.Add(group);
}

{
    var group = new Group();
    group.Name = "My new resource group";
    group.MaintainHierarchy = true;
    group.ShowSummary = true;

    var criterion = new GroupCriterion();
    criterion.Field = Field.ResourceDuration1;
    criterion.Font = new FontDescriptor("Comic Sans MS", 11F, FontStyles.Bold);
    criterion.GroupOn = GroupOn.DurationHours;
    criterion.StartAt = 1;
    criterion.GroupInterval = 2D;
    criterion.Pattern = BackgroundPattern.DarkDiagonalLeft;
    group.GroupCriteria.Add(criterion);

    var criterion2 = new GroupCriterion();
    criterion2.Field = Field.ResourceCost;
    criterion2.Font = new FontDescriptor("Bodoni MT", 12, FontStyles.Italic | FontStyles.Bold);
    criterion2.GroupOn = GroupOn.Interval;
    criterion2.StartAt = 1D;
    criterion2.GroupInterval = 10D;
    criterion2.Pattern = BackgroundPattern.LightDither;
    criterion2.CellColor = Color.Magenta;
    criterion2.FontColor = Color.Red;
    group.GroupCriteria.Add(criterion2);
    group.GroupAssignments = true;
    p.ResourceGroups.Add(group);
}

p.Save(OutDir + "output_CreateGroup.mpp", new MPPSaveOptions() { WriteGroups = true });
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



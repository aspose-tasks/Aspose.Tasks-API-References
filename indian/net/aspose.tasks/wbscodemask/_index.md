---
title: "`WBSCodeMask` वर्ग"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "`Aspose.Tasks.WBSCodeMask` वर्ग। यह WBS कोड मास्क का प्रतिनिधित्व करता है।"
type: docs
weight: 3500
url: /hi/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

WBS कोड मास्क दर्शाता है।

```csharp
public class WBSCodeMask
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | `WBSCodeMask` वर्ग का नया उदाहरण प्रारंभ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | कोड स्ट्रिंग के अक्षरों की संख्या को प्राप्त करता है या सेट करता है। |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | मास्क स्तर प्राप्त करता है। |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | कोड स्ट्रिंग के विभाजक को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान अवधि है। |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | कोड स्ट्रिंग के अक्षर प्रकार को प्राप्त करता है या सेट करता है। |

## उदाहरण

WBS कोड मास्क बनाने का तरीका दिखाता है।

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



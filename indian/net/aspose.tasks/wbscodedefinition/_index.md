---
title: "क्लास WBSCodeDefinition"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.WBSCodeDefinition क्लास। एक WBS कोड परिभाषा का प्रतिनिधित्व करता है"
type: docs
weight: 3490
url: /hi/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

WBS कोड परिभाषा दर्शाता है।

```csharp
public class WBSCodeDefinition
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | `WBSCodeDefinition` क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | WBSCodeMask ऑब्जेक्ट्स का संग्रह प्राप्त करता है। |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | प्रोजेक्ट कोड उपसर्ग को प्राप्त करता है या सेट करता है। |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | नए कार्य के लिए WBS कोड उत्पन्न करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | नए WBS कोड की विशिष्टता की जाँच करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |

## उदाहरण

WBS कोड मास्क जोड़ने का तरीका दिखाता है।

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

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



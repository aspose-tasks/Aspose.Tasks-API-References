---
title: "WBSCodeMask.Sequence"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WBSCodeMask प्रॉपर्टी। कोड स्ट्रिंग के अक्षर प्रकार को प्राप्त करता है या सेट करता है"
type: docs
weight: 50
url: /hi/net/aspose.tasks/wbscodemask/sequence/
---
## WBSCodeMask.Sequence property

कोड स्ट्रिंग के अक्षर प्रकार को प्राप्त करता है या सेट करता है।

```csharp
public WBSSequence Sequence { get; set; }
```

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

* enum [WBSSequence](../../wbssequence/)
* class [WBSCodeMask](../)
* namespace [Aspose.Tasks](../../wbscodemask/)
* assembly [Aspose.Tasks](../../../)



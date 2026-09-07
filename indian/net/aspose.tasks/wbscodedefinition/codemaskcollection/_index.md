---
title: "WBSCodeDefinition.CodeMaskCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WBSCodeDefinition प्रॉपर्टी। WBSCodeMask ऑब्जेक्ट्स का संग्रह प्राप्त करता है"
type: docs
weight: 20
url: /hi/net/aspose.tasks/wbscodedefinition/codemaskcollection/
---
## WBSCodeDefinition.CodeMaskCollection property

WBSCodeMask ऑब्जेक्ट्स का संग्रह प्राप्त करता है।

```csharp
public WBSCodeMaskCollection CodeMaskCollection { get; }
```

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

* class [WBSCodeMaskCollection](../../wbscodemaskcollection/)
* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)



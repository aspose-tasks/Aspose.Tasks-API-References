---
title: "WBSCodeDefinition.GenerateWBSCode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WBSCodeDefinition प्रॉपर्टी। नई कार्य के लिए WBS कोड उत्पन्न करने का संकेत देने वाला मान प्राप्त या सेट करता है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/wbscodedefinition/generatewbscode/
---
## WBSCodeDefinition.GenerateWBSCode property

नए कार्य के लिए WBS कोड उत्पन्न करने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है।

```csharp
public bool GenerateWBSCode { get; set; }
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

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)



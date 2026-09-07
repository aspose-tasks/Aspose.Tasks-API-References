---
title: "WBSCodeDefinition.CodePrefix"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "WBSCodeDefinition प्रॉपर्टी। प्रोजेक्ट कोड उपसर्ग प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.tasks/wbscodedefinition/codeprefix/
---
## WBSCodeDefinition.CodePrefix property

प्रोजेक्ट कोड उपसर्ग को प्राप्त करता है या सेट करता है।

```csharp
public string CodePrefix { get; set; }
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



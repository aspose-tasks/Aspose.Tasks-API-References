---
title: "WBSCodeDefinition.WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WBSCodeDefinition yapıcı. WBSCodeDefinition sınıfının yeni bir örneğini başlatır."
type: docs
weight: 10
url: /tr/net/aspose.tasks/wbscodedefinition/wbscodedefinition/
---
## WBSCodeDefinition constructor

[`WBSCodeDefinition`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public WBSCodeDefinition()
```

## Örnekler

WBS kod maskeleri eklemenin nasıl yapılacağını gösterir.

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

### Ayrıca Bakınız

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)



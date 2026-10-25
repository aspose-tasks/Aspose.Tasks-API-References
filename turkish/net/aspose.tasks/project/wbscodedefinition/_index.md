---
title: "Project.WBSCodeDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. Proje için WBS Code Definition değerini alır veya ayarlar"
type: docs
weight: 1030
url: /tr/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

Proje için WBS Kod Tanımını alır veya ayarlar.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## Örnekler

WBS kodlarının nasıl ekleneceğini gösterir.

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)



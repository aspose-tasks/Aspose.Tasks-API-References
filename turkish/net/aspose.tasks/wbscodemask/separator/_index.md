---
title: "WBSCodeMask.Separator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "WBSCodeMask özelliği. Kod dizesinin ayırıcı karakterini alır veya ayarlar. Varsayılan değer Period'dur"
type: docs
weight: 40
url: /tr/net/aspose.tasks/wbscodemask/separator/
---
## WBSCodeMask.Separator property

Kod dizesinin ayırıcı değerini alır veya ayarlar. Varsayılan değer Nokta'dır.

```csharp
public string Separator { get; set; }
```

## Örnekler

WBS kod maskelerinin nasıl oluşturulacağını gösterir.

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

### Ayrıca Bakınız

* class [WBSCodeMask](../)
* namespace [Aspose.Tasks](../../wbscodemask/)
* assembly [Aspose.Tasks](../../../)



---
title: "WBSCodeMask Sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WBSCodeMask sınıfı. WBS Kod maskesini temsil eder."
type: docs
weight: 3500
url: /tr/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

WBS Kod maskesini temsil eder.

```csharp
public class WBSCodeMask
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | `WBSCodeMask` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | Kod dizesinin karakter sayısını alır veya ayarlar. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | Maskenin seviyesini alır. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | Kod dizesinin ayırıcı değerini alır veya ayarlar. Varsayılan değer Nokta'dır. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | Kod dizesinin karakter tipini alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



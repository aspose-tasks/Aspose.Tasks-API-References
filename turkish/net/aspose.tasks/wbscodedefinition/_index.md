---
title: "WBSCodeDefinition sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.WBSCodeDefinition sınıfı. Bir WBS Kod Tanımını temsil eder"
type: docs
weight: 3490
url: /tr/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

Bir WBS Kod Tanımını temsil eder.

```csharp
public class WBSCodeDefinition
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | `WBSCodeDefinition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | WBSCodeMask nesnelerinin koleksiyonunu alır. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | Proje kodu önekini alır veya ayarlar. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | Yeni görev için WBS kodu oluşturulup oluşturulmayacağını belirten bir değeri alır veya ayarlar. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | Yeni WBS kodlarının benzersizliğinin doğrulanıp doğrulanmayacağını belirten bir değeri alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



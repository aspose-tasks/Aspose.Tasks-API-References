---
title: "Enum CustomFieldType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.CustomFieldType enum. Özel bir alanın türünü belirtir."
type: docs
weight: 380
url: /tr/net/aspose.tasks/customfieldtype/
---
## CustomFieldType enumeration

Özel alanın tipini belirtir.

```csharp
public enum CustomFieldType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Null | `0` | Null özel alan türünü gösterir. |
| Cost | `1` | Maliyet özel alan türünü gösterir. |
| Date | `2` | Tarih özel alan türünü gösterir. |
| Duration | `3` | Süre özel alan türünü gösterir. |
| Finish | `4` | Bitiş özel alan türünü gösterir. |
| Flag | `5` | Bayrak özel alan türünü gösterir. |
| Number | `6` | Numara özel alan türünü gösterir. |
| Start | `7` | Başlangıç özel alan türünü gösterir. |
| Text | `8` | Metin özel alan türünü gösterir. |
| OutlineCode | `9` | Anahat Kodu özel alan türünü gösterir. |
| RBS | `10` | RBS (Kaynak Ayrıntı Yapısı) özel alan türünü gösterir. |

## Örnekler

&lt;see cref=\"CustomFieldType\" /&gt; (CustomFieldType.Text) nasıl kullanılacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text1,
    "MyText");
project.ExtendedAttributes.Add(definition);
// tanımlarla çalış...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



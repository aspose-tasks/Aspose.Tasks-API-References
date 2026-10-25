---
title: "Sınıf OutlineMask"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineMask sınıfı. Bir taslak kod formatını tanımlayan maskenin dört öğesini temsil eder."
type: docs
weight: 1190
url: /tr/net/aspose.tasks/outlinemask/
---
## OutlineMask class

Bir ana hat kodu biçimini tanımlayan maskenin dört öğesini temsil eder.

```csharp
public class OutlineMask
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OutlineMask](outlinemask/)() | Yeni bir `OutlineMask` sınıfı örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Length](../../aspose.tasks/outlinemask/length/) { get; set; } | Taslak kod değerlerinin maksimum uzunluğunu (karakter cinsinden) alır veya ayarlar. Uzunluk tanımlı değilse 0. |
| [Level](../../aspose.tasks/outlinemask/level/) { get; set; } | Bir maskenin seviyesini alır veya ayarlar. |
| [Separator](../../aspose.tasks/outlinemask/separator/) { get; set; } | Kod değerlerinin ayıracısını alır veya ayarlar. |
| [Type](../../aspose.tasks/outlinemask/type/) { get; set; } | Maskenin türünü alır veya ayarlar. |

## Örnekler

Ana hat maskeleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();

// maskenin türünü ayarla
mask.Type = MaskType.Characters;

// kod değerlerinin ayıracısını ayarla
mask.Separator = "/";

// maskenin seviyesini ayarla
mask.Level = 1;

// ana hat kod değerlerinin maksimum uzunluğunu (karakter cinsinden) ayarla. Uzunluk tanımlı değilse 0.
mask.Length = 2;

// maskeyi tanıma ekle
outline.Masks.Add(mask);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



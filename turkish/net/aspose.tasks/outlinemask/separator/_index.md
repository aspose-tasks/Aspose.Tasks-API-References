---
title: "OutlineMask.Separator"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineMask özelliği. Kod değerlerinin ayıracısını alır veya ayarlar."
type: docs
weight: 40
url: /tr/net/aspose.tasks/outlinemask/separator/
---
## OutlineMask.Separator property

Kod değerlerinin ayıracısını alır veya ayarlar.

```csharp
public string Separator { get; set; }
```

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

* class [OutlineMask](../)
* namespace [Aspose.Tasks](../../outlinemask/)
* assembly [Aspose.Tasks](../../../)



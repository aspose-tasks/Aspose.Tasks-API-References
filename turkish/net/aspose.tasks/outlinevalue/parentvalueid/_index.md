---
title: "OutlineValue.ParentValueId"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineValue özelliği. Outline kodunun bir üst düğümünün kimliğini alır veya ayarlar."
type: docs
weight: 50
url: /tr/net/aspose.tasks/outlinevalue/parentvalueid/
---
## OutlineValue.ParentValueId property

Bir taslak kodunun üst düğümünün kimliğini alır veya ayarlar.

```csharp
public int ParentValueId { get; set; }
```

## Örnekler

Taslak değerlerle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

var outline = new OutlineCodeDefinition();
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline.Alias = "My Outline Code";
var outline2 = new OutlineCodeDefinition();
outline2.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");
outline2.Alias = "My Outline Code 2";

project.OutlineCodes.Add(outline);

var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// bir taslak değer oluştur
var value = new OutlineValue();

// gerçek değeri ayarla
value.Value = "Text value 1";

// bir proje içinde taslak kod değerinin benzersiz kimliğini ayarla
value.ValueId = 1;

// tüm projedeki diğer değerler arasında bu değeri tanımlayan bir GUID al
Console.WriteLine("Check value GUID: " + value.ValueGuid);

// taslak kod türünü ayarla
value.Type = OutlineValueType.Text;

// taslak değerin açıklamasını ayarla
value.Description = "Text value descr 1";

// taslak değerin daraltılmış olup olmadığını gösteren bir değer ayarla
value.IsCollapsed = false;

// üst değer kimliğini kontrol et
Console.WriteLine("Check parent value id: " + value.ParentValueId);
outline.Values.Add(value);

// süre ile bir taslak değer oluştur
var value2 = new OutlineValue();

// süre değerini ayarla
value2.DurationValue = project.GetDuration(1, TimeUnitType.Hour);

// bir proje içinde taslak kod değerinin benzersiz kimliğini ayarla
value2.ValueId = 2;
outline2.Values.Add(value2);

// ...
```

### Ayrıca Bakınız

* class [OutlineValue](../)
* namespace [Aspose.Tasks](../../outlinevalue/)
* assembly [Aspose.Tasks](../../../)



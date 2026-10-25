---
title: "OutlineCodeDefinition.LeafOnly"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "OutlineCodeDefinition özelliği. Bu ana hat kodu alanında belirtilen değerlerin yaprak değerler olması gerekip gerekmediğini gösteren bir değeri alır veya ayarlar"
type: docs
weight: 90
url: /tr/net/aspose.tasks/outlinecodedefinition/leafonly/
---
## OutlineCodeDefinition.LeafOnly property

Bu outline kod alanında belirtilen değerlerin yaprak değerler olması gerekip gerekmediğini gösteren bir değeri alır veya ayarlar.

```csharp
public bool LeafOnly { get; set; }
```

## Örnekler

Ana hat kodu tanımlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// yeni bir ana hat kodu tanımı oluştur
var outline = new OutlineCodeDefinition();

// bir ana hat kodunun alan numarasını ayarla
outline.FieldId = ExtendedAttributeTask.OutlineCode7.ToString("D");

// özel bir ana hat kodunun adını ayarla
outline.FieldName = "Outline Code1";

// bir ana hat kodunun Guid'ini ayarla
outline.Guid = "e6afac06-0d86-4359-a96c-db705e3d2ca8";

// bu ana hat kodu alanında belirtilen değerlerin yaprak değerler olması gerekip gerekmediğini gösteren bir değer ayarla
outline.LeafOnly = false;

// özel bir ana hat kodunun takma adını ayarla
outline.Alias = "My Outline Code";

// özel ana hat kodunun takma adının fonetik telaffuzunu ayarla
outline.PhoneticAlias = "Outline Code";

// yeni kodların tüm seviyelere sahip olması gerekip gerekmediğini gösteren bir değer ayarla. Kurumsal Kodlar için mevcut değildir.
outline.AllLevelsRequired = true;

// özel bir ana hat kodunun kurumsal özel bir ana hat kodu olup olmadığını gösteren bir değer ayarla
outline.Enterprise = false;

// bu ana hat kodu tanımının takma adı olduğu başka bir özel alana referans ayarla
outline.EnterpriseOutlineCodeAlias = 0;

// bir ana hat maskesi ekle
var mask = new OutlineMask();
mask.Type = MaskType.Characters;
outline.Masks.Add(mask);

// belirtilen değerlerin değerler tablosundan gelmesi gerekip gerekmediğini gösteren bir değer ayarla
outline.OnlyTableValuesAllowed = false;

// özel ana hat kodunun kullanılabilir olup olmadığını gösteren bir değer ayarla
// Microsoft Project'teki Kaynak Değiştirme Sihirbazı tarafından
outline.ResourceSubstitutionEnabled = false;

// bu ana hat kodunun girintilerinin gösterilip gösterilmeyeceğini belirten bir değer ayarla.
outline.ShowIndent = false;

project.OutlineCodes.Add(outline);

var value = new OutlineValue();
value.Value = "Text value 1";
value.ValueId = 1;
value.Type = OutlineValueType.Text;
value.Description = "Text value descr 1";
outline.Values.Add(value);

// ...
```

### Ayrıca Bakınız

* class [OutlineCodeDefinition](../)
* namespace [Aspose.Tasks](../../outlinecodedefinition/)
* assembly [Aspose.Tasks](../../../)



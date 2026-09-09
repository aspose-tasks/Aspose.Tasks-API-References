---
title: "Sınıf OutlineCodeDefinition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.OutlineCodeDefinition sınıfı. Bir outline kod tanımını temsil eder."
type: docs
weight: 1170
url: /tr/net/aspose.tasks/outlinecodedefinition/
---
## OutlineCodeDefinition class

Bir ana hat kodu tanımını temsil eder.

```csharp
public sealed class OutlineCodeDefinition
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [OutlineCodeDefinition](outlinecodedefinition/)() | `OutlineCodeDefinition` sınıfının yeni bir örneğini başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Alias](../../aspose.tasks/outlinecodedefinition/alias/) { get; set; } | Özel bir outline kodunun takma adını alır veya ayarlar. |
| [AllLevelsRequired](../../aspose.tasks/outlinecodedefinition/alllevelsrequired/) { get; set; } | Yeni kodların tüm seviyelere sahip olup olmadığını gösteren bir değeri alır veya ayarlar. Enterprise Kodları için mevcut değildir. |
| [Enterprise](../../aspose.tasks/outlinecodedefinition/enterprise/) { get; set; } | Özel bir outline kodunun kurumsal özel outline kodu olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [EnterpriseOutlineCodeAlias](../../aspose.tasks/outlinecodedefinition/enterpriseoutlinecodealias/) { get; set; } | Bu outline kod tanımının takma adı olduğu başka bir özel alana referansı alır veya ayarlar. |
| [FieldId](../../aspose.tasks/outlinecodedefinition/fieldid/) { get; set; } | Bir outline kodunun alan numarasını alır veya ayarlar. |
| [FieldName](../../aspose.tasks/outlinecodedefinition/fieldname/) { get; set; } | Özel bir outline kodunun adını alır veya ayarlar. |
| [Guid](../../aspose.tasks/outlinecodedefinition/guid/) { get; set; } | Bir outline kodunun GUID'ini alır veya ayarlar. |
| [LeafOnly](../../aspose.tasks/outlinecodedefinition/leafonly/) { get; set; } | Bu outline kod alanında belirtilen değerlerin yaprak değerler olması gerekip gerekmediğini gösteren bir değeri alır veya ayarlar. |
| [Masks](../../aspose.tasks/outlinecodedefinition/masks/) { get; } | OutlineMaskCollection nesnesini alır. Outline kod maskesini tanımlayan girişlerin tablosu. Salt okunur [`OutlineMaskCollection`](../outlinemaskcollection/) örneği. |
| [OnlyTableValuesAllowed](../../aspose.tasks/outlinecodedefinition/onlytablevaluesallowed/) { get; set; } | Belirtilen değerlerin değerler tablosundan gelmesi gerekip gerekmediğini gösteren bir değeri alır veya ayarlar. |
| [PhoneticAlias](../../aspose.tasks/outlinecodedefinition/phoneticalias/) { get; set; } | Özel outline kodunun takma adının fonetik telaffuzunu alır veya ayarlar. |
| [ResourceSubstitutionEnabled](../../aspose.tasks/outlinecodedefinition/resourcesubstitutionenabled/) { get; set; } | Özel outline kodunun Microsoft Project'teki Kaynak Değiştirme Sihirbazı tarafından kullanılabilir olup olmadığını gösteren bir değeri alır veya ayarlar. |
| [ShowIndent](../../aspose.tasks/outlinecodedefinition/showindent/) { get; set; } | Bu outline kodunun girintilerinin gösterilmesi gerekip gerekmediğini gösteren bir değeri alır veya ayarlar. |
| [Values](../../aspose.tasks/outlinecodedefinition/values/) { get; } | OutlineValueCollection nesnesini alır. Bu ana hat koduyla ilişkili tablonun değerleri. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



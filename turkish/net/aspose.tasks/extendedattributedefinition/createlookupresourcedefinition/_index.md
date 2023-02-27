---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: ExtendedAttributeDefinition yöntem. Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemiCalculationType eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekiyorfieldId Vealias bu yöntem çağrıldığında. Alan türü id. alanından çıkarılır.
type: docs
weight: 10
url: /tr/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](../calculationtype/) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Belirtilen[`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*fieldId* Ve*alias*.

### Örnekler

Aramalı bir kaynak için özel bir alan tanımı oluşturmak ve ardından bunu metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ayrıca bakınız

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](../calculationtype/) eşittirLookup ve yalnızca Kaynaklarda kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen[`CustomFieldType`](../../customfieldtype/) tip. |
| fieldId | ExtendedAttributeResource | Belirtilen[`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*customFieldType* ,*fieldId* Ve*alias*.

### Örnekler

Aramalı bir kaynak için özel bir alan tanımı oluşturmak ve ardından bunu metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ayrıca bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)



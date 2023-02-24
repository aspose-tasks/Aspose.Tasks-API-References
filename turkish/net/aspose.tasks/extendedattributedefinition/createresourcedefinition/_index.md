---
title: ExtendedAttributeDefinition.CreateResourceDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: ExtendedAttributeDefinition yöntem. Microsoft Projectin Yok olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. CalculationType eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekiyorcustomFieldType fieldId Vealias bu yöntemi çağırdığınızda.
type: docs
weight: 30
url: /tr/net/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---
## CreateResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createresourcedefinition}

Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen[`CustomFieldType`](../../customfieldtype/) tip. |
| fieldId | ExtendedAttributeResource | Belirtilen[`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*customFieldType* ,*fieldId* Ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ayrıca bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)

---

## CreateResourceDefinition(ExtendedAttributeResource, string) {#createresourcedefinition_1}

Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) eşittirNone ve yalnızca Kaynakta kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Belirtilen[`ExtendedAttributeResource`](../../extendedattributeresource/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*fieldId* Ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Ayrıca bakınız

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)



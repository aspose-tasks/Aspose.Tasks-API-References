---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: ExtendedAttributeDefinition yöntem. Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemiCalculationType eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyorfieldId Vealias bu yöntem çağrıldığında. Alan türü id. alanından çıkarılır.
type: docs
weight: 20
url: /tr/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](../calculationtype/) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntem çağrıldığında. Alan türü, id. alanından çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Belirtilen[`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*fieldId* Ve*alias*.

### Örnekler

Aramalı bir görev için özel bir alan tanımı oluşturmak ve ardından bunu metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Lookup. ile genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi[`CalculationType`](../calculationtype/) eşittirLookup ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırdığınızda.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen[`CustomFieldType`](../../customfieldtype/) tip. |
| fieldId | ExtendedAttributeTask | Belirtilen[`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*customFieldType* ,*fieldId* Ve*alias*.

### Örnekler

Aramalı bir görev için özel bir alan tanımı oluşturmak ve ardından bunu metin değerleriyle doldurmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)



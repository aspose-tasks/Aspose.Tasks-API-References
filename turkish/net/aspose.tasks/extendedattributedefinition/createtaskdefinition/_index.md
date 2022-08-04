---
title: CreateTaskDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: Microsoft Projectin Yok olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. CalculationTypeaspose.tasks/extendedattributedefinition/calculationtype eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekircustomFieldType fieldId vealias bu yöntemi çağırırken.
type: docs
weight: 40
url: /tr/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*customFieldType* ,*fieldId* ve*alias* bu yöntemi çağırırken.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilmiş[`CustomFieldType`](../../customfieldtype) tip. |
| fieldId | ExtendedAttributeTask | Belirtilmiş[`ExtendedAttributeTask`](../../extendedattributetask) alan kimliği. |
| alias | String | BelirtilmişString takma ad. |

### Geri dönüş değeri

Oluşturulan örneği[`ExtendedAttributeDefinition`](../../extendedattributedefinition) belirtilen sınıf*customFieldType* ,*fieldId* ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [CustomFieldType](../../customfieldtype)
* enum [ExtendedAttributeTask](../../extendedattributetask)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition)
* toplantı [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Microsoft Project'in "Yok" olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekir*fieldId* ve*alias* bu yöntemi çağırırken. Alan türü, alan kimliğinden çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Belirtilmiş[`ExtendedAttributeTask`](../../extendedattributetask) alan kimliği. |
| alias | String | BelirtilmişString takma ad. |

### Geri dönüş değeri

Oluşturulan örneği[`ExtendedAttributeDefinition`](../../extendedattributedefinition) belirtilen sınıf*fieldId* ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [ExtendedAttributeTask](../../extendedattributetask)
* class [ExtendedAttributeDefinition](../../extendedattributedefinition)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition)
* toplantı [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Aspose.Tasks for .NET API Referansı
description: ExtendedAttributeDefinition yöntem. Microsoft Projectin Yok olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. CalculationType eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyorcustomFieldType fieldId Vealias bu yöntemi çağırırken.
type: docs
weight: 40
url: /tr/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*customFieldType* ,*fieldId* Ve*alias* bu yöntemi çağırırken.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| customFieldType | CustomFieldType | Belirtilen[`CustomFieldType`](../../customfieldtype/) tip. |
| fieldId | ExtendedAttributeTask | Belirtilen[`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*customFieldType* ,*fieldId* Ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Microsoft Project'in "Yok" olarak gösterdiği, basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi. [`CalculationType`](../calculationtype/) eşittirNone ve yalnızca Görevlerde kullanılabilir. Belirtmeniz gerekiyor*fieldId* Ve*alias* bu yöntemi çağırırken. Alan türü, id. alanından çıkarılır.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Belirtilen[`ExtendedAttributeTask`](../../extendedattributetask/) alan kimliği. |
| alias | String | BelirtilenString takma ad. |

### Geri dönüş değeri

Oluşturulan örnek[`ExtendedAttributeDefinition`](../) belirtilen sınıf*fieldId* Ve*alias*.

### Örnekler

Özel bir metin alanı tanımı oluşturmak için bu örneği kullanın:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### Ayrıca bakınız

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* ad alanı [Aspose.Tasks](../../extendedattributedefinition/)
* toplantı [Aspose.Tasks](../../../)



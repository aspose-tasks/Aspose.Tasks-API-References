---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Aspose.Tasks لمرجع .NET API
description: ExtendedAttributeDefinition طريقة. طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطًا  والذي يظهره Microsoft Project على أنه بلا. يحتوي علىCalculationType يساويNone ويمكن استخدامها في المهام فقط. أنت مطالب بالتحديدcustomFieldType وfieldId وalias عند استدعاء هذه الطريقة.
type: docs
weight: 40
url: /ar/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطًا ، والذي يظهره Microsoft Project على أنه "بلا". يحتوي على[`CalculationType`](../calculationtype/) يساويNone ويمكن استخدامها في المهام فقط. أنت مطالب بالتحديد*customFieldType* و*fieldId* و*alias* عند استدعاء هذه الطريقة.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| customFieldType | CustomFieldType | المحدد[`CustomFieldType`](../../customfieldtype/) يكتب. |
| fieldId | ExtendedAttributeTask | المحدد[`ExtendedAttributeTask`](../../extendedattributetask/) معرف المجال. |
| alias | String | المحددString الاسم المستعار. |

### قيمة الإرجاع

تم إنشاء مثيل لـ[`ExtendedAttributeDefinition`](../) فئة مع المحدد*customFieldType* و*fieldId* و*alias*.

### أمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### أنظر أيضا

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* مساحة الاسم [Aspose.Tasks](../../extendedattributedefinition/)
* المجسم [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

طريقة المصنع التي تنشئ تعريف سمة موسعة بسيطًا ، والذي يظهره Microsoft Project على أنه "بلا". يحتوي على[`CalculationType`](../calculationtype/) يساويNone ويمكن استخدامها في المهام فقط. أنت مطالب بالتحديد*fieldId* و*alias* عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من معرف الحقل.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | المحدد[`ExtendedAttributeTask`](../../extendedattributetask/) معرف المجال. |
| alias | String | المحددString الاسم المستعار. |

### قيمة الإرجاع

تم إنشاء مثيل لـ[`ExtendedAttributeDefinition`](../) فئة مع المحدد*fieldId* و*alias*.

### أمثلة

استخدم هذا المثال لإنشاء تعريف حقل نص مخصص:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

### أنظر أيضا

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* مساحة الاسم [Aspose.Tasks](../../extendedattributedefinition/)
* المجسم [Aspose.Tasks](../../../)



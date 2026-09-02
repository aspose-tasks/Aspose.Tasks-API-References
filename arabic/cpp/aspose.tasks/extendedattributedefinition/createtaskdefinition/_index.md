---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition طريقة"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks لـ C++"
description: "طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، والذي يظهر في Microsoft Project كـ \"None\"."
type: docs
weight: 60
url: /ar/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

طريقة مصنع تقوم بإنشاء تعريف سمة موسعة بسيطة، التي يعرضها Microsoft Project كـ "None". لديها CalculationType تساوي Tasks::CalculationType::None ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد customFieldType و fieldId و alias عند استدعاء هذه الطريقة.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| customFieldType | نوع CustomFieldType المحدد. |
| fieldId | معرف الحقل ExtendedAttributeTask المحدد. |
| alias | الاسم المستعار System::String المحدد. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، والذي يظهر في Microsoft Project كـ "None". لديها CalculationType تساوي Tasks::CalculationType::None ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد fieldId و alias عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من معرف الحقل.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| fieldId | معرف الحقل ExtendedAttributeTask المحدد. |
| alias | الاسم المستعار System::String المحدد. |


---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition طريقة"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks لـ C++"
description: "طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، والذي يظهر في Microsoft Project كـ \"None\"."
type: docs
weight: 50
url: /ar/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

طريقة مصنع تقوم بإنشاء تعريف سمة موسعة بسيطة، التي يعرضها Microsoft Project كـ "None". لديها CalculationType تساوي Tasks::CalculationType::None ويمكن استخدامها في Resource فقط. يُطلب منك تحديد customFieldType و fieldId و alias عند استدعاء هذه الطريقة.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| customFieldType | نوع CustomFieldType المحدد. |
| fieldId | معرف الحقل ExtendedAttributeResource المحدد. |
| alias | الاسم المستعار System::String المحدد. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

طريقة المصنع التي تنشئ تعريف سمة موسعة بسيط، والذي يظهر في Microsoft Project كـ "None". لديها CalculationType تساوي Tasks::CalculationType::None ويمكن استخدامها في الموارد فقط. يجب عليك تحديد fieldId و alias عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| fieldId | معرف الحقل ExtendedAttributeResource المحدد. |
| alias | الاسم المستعار System::String المحدد. |


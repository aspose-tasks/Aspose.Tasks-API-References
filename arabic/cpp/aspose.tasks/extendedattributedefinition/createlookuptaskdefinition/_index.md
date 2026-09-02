---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition طريقة"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks لـ C++"
description: "طريقة المصنع التي تنشئ تعريف خاصية موسعة مع البحث."
type: docs
weight: 40
url: /ar/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

طريقة مصنع تقوم بإنشاء تعريف سمة موسعة مع بحث. لديها CalculationType تساوي Tasks::CalculationType::Lookup ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد customFieldType و fieldId و alias عند استدعاء هذه الطريقة.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| customFieldType | نوع CustomFieldType المحدد. |
| fieldId | معرف الحقل ExtendedAttributeTask المحدد. |
| alias | الاسم المستعار System::String المحدد. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

طريقة المصنع التي تنشئ تعريف سمة موسعة مع بحث. لديها CalculationType تساوي Tasks::CalculationType::Lookup ويمكن استخدامها في Tasks فقط. يُطلب منك تحديد fieldId و alias عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من معرف الحقل.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| fieldId | معرف الحقل ExtendedAttributeTask المحدد. |
| alias | الاسم المستعار System::String المحدد. |


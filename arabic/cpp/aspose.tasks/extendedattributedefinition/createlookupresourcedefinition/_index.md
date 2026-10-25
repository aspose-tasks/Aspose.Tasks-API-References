---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition طريقة"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks لـ C++"
description: "طريقة المصنع التي تنشئ تعريف خاصية موسعة مع البحث."
type: docs
weight: 30
url: /ar/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

طريقة مصنع تقوم بإنشاء تعريف سمة موسعة مع بحث. لديها CalculationType تساوي Tasks::CalculationType::Lookup ويمكن استخدامها في Resources فقط. يُطلب منك تحديد customFieldType و fieldId و alias عند استدعاء هذه الطريقة.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| customFieldType | نوع CustomFieldType المحدد. |
| fieldId | معرف الحقل ExtendedAttributeResource المحدد. |
| alias | الاسم المستعار System::String المحدد. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

طريقة المصنع التي تنشئ تعريف خاصية موسعة مع البحث. لها CalculationType تساوي Tasks::CalculationType::Lookup ولا يمكن استخدامها إلا في Resources. يتوجب عليك تحديد fieldId و alias عند استدعاء هذه الطريقة. يتم استنتاج نوع الحقل من field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| معامل | الوصف |
| --- | --- |
| fieldId | معرف الحقل ExtendedAttributeResource المحدد. |
| alias | الاسم المستعار System::String المحدد. |


---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition metodu"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "C++ için Aspose.Tasks"
description: "Arama ile genişletilmiş öznitelik tanımı oluşturan fabrika metodu."
type: docs
weight: 30
url: /tr/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::Lookup'e eşittir ve yalnızca Kaynaklarda kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| customFieldType | Belirtilen CustomFieldType türü. |
| fieldId | Belirtilen ExtendedAttributeResource alan kimliği. |
| alias | Belirtilen System::String takma adı. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Arama ile genişletilmiş öznitelik tanımı oluşturan fabrika metodu. CalculationType değeri Tasks::CalculationType::Lookup olarak ayarlanmıştır ve yalnızca Resources içinde kullanılabilir. Bu metodu çağırdığınızda fieldId ve alias belirtmeniz gerekir. Alan türü field id'den çıkarılır.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| fieldId | Belirtilen ExtendedAttributeResource alan kimliği. |
| alias | Belirtilen System::String takma adı. |


---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition metodu"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "C++ için Aspose.Tasks"
description: "Arama ile genişletilmiş öznitelik tanımı oluşturan fabrika metodu."
type: docs
weight: 40
url: /tr/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Arama ile genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::Lookup'e eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| customFieldType | Belirtilen CustomFieldType türü. |
| fieldId | Belirtilen ExtendedAttributeTask alan kimliği. |
| alias | Belirtilen System::String takma adı. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Lookup ile bir genişletilmiş öznitelik tanımı oluşturan fabrika metodu. CalculationType değeri Tasks::CalculationType::Lookup'tir ve yalnızca Tasks içinde kullanılabilir. Bu metodu çağırırken fieldId ve alias belirtmeniz gerekir. Alan türü field id'den çıkarılır.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| fieldId | Belirtilen ExtendedAttributeTask alan kimliği. |
| alias | Belirtilen System::String takma adı. |


---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition metodu"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "C++ için Aspose.Tasks"
description: "Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika metodu, Microsoft Project'in \"None\" olarak gösterdiği."
type: docs
weight: 60
url: /tr/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::None'a eşittir ve yalnızca Görevlerde kullanılabilir. Bu yöntemi çağırırken customFieldType, fieldId ve alias belirtmeniz gerekir.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| customFieldType | Belirtilen CustomFieldType türü. |
| fieldId | Belirtilen ExtendedAttributeTask alan kimliği. |
| alias | Belirtilen System::String takma adı. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika metodu, Microsoft Project'in "None" olarak gösterdiği. CalculationType değeri Tasks::CalculationType::None'dir ve yalnızca Tasks içinde kullanılabilir. Bu metodu çağırırken fieldId ve alias belirtmeniz gerekir. Alan türü field id'den çıkarılır.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| fieldId | Belirtilen ExtendedAttributeTask alan kimliği. |
| alias | Belirtilen System::String takma adı. |


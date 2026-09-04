---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition metodu"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "C++ için Aspose.Tasks"
description: "Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika metodu, Microsoft Project'in \"None\" olarak gösterdiği."
type: docs
weight: 50
url: /tr/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Microsoft Project'in \"None\" (Yok) olarak gösterdiği basit bir genişletilmiş öznitelik tanımı oluşturan bir fabrika yöntemi. CalculationType'ı Tasks::CalculationType::None'a eşittir ve yalnızca Kaynakta kullanılabilir. Bu yöntemi çağırdığınızda customFieldType, fieldId ve alias belirtmeniz gerekir.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| customFieldType | Belirtilen CustomFieldType türü. |
| fieldId | Belirtilen ExtendedAttributeResource alan kimliği. |
| alias | Belirtilen System::String takma adı. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Basit bir genişletilmiş öznitelik tanımı oluşturan fabrika yöntemi, Microsoft Project'in "None" olarak gösterdiği. CalculationType değeri Tasks::CalculationType::None olarak ayarlanmıştır ve yalnızca Resource içinde kullanılabilir. Bu yöntemi çağırdığınızda fieldId ve alias belirtmeniz gerekir. Alan türü field id'den türetilir.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametre | Açıklama |
| --- | --- |
| fieldId | Belirtilen ExtendedAttributeResource alan kimliği. |
| alias | Belirtilen System::String takma adı. |


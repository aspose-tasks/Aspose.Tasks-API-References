---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition метод"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks для C++"
description: "Фабричный метод, который создаёт определение расширенного атрибута с поиском."
type: docs
weight: 30
url: /ru/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Фабричный метод, который создаёт определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в ресурсах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| customFieldType | Указанный тип CustomFieldType. |
| fieldId | Указанный идентификатор поля ExtendedAttributeResource. |
| alias | Указанный псевдоним System::String. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Фабричный метод, который создает определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в Resources. Требуется указать fieldId и alias при вызове этого метода. Тип поля выводится из fieldId.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| fieldId | Указанный идентификатор поля ExtendedAttributeResource. |
| alias | Указанный псевдоним System::String. |


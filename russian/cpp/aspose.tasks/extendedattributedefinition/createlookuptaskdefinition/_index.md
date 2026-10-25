---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition метод"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks для C++"
description: "Фабричный метод, который создаёт определение расширенного атрибута с поиском."
type: docs
weight: 40
url: /ru/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Фабричный метод, который создаёт определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в задачах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| customFieldType | Указанный тип CustomFieldType. |
| fieldId | Указанный идентификатор поля ExtendedAttributeTask. |
| alias | Указанный псевдоним System::String. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Фабричный метод, который создает определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в Tasks. Требуется указать fieldId и alias при вызове этого метода. Тип поля выводится из fieldId.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| fieldId | Указанный идентификатор поля ExtendedAttributeTask. |
| alias | Указанный псевдоним System::String. |


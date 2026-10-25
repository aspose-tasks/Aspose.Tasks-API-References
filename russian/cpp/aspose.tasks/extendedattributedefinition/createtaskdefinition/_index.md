---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition метод"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks для C++"
description: "Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\"."
type: docs
weight: 60
url: /ru/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Фабричный метод, который создаёт простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в задачах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| customFieldType | Указанный тип CustomFieldType. |
| fieldId | Указанный идентификатор поля ExtendedAttributeTask. |
| alias | Указанный псевдоним System::String. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в Tasks. Требуется указать fieldId и alias при вызове этого метода. Тип поля выводится из fieldId.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| fieldId | Указанный идентификатор поля ExtendedAttributeTask. |
| alias | Указанный псевдоним System::String. |


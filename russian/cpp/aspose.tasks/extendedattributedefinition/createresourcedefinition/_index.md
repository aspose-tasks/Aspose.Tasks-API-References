---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition метод"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks для C++"
description: "Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\"."
type: docs
weight: 50
url: /ru/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Фабричный метод, который создаёт простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в ресурсах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| customFieldType | Указанный тип CustomFieldType. |
| fieldId | Указанный идентификатор поля ExtendedAttributeResource. |
| alias | Указанный псевдоним System::String. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в Resource. Требуется указать fieldId и alias при вызове этого метода. Тип поля выводится из fieldId.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Параметр | Описание |
| --- | --- |
| fieldId | Указанный идентификатор поля ExtendedAttributeResource. |
| alias | Указанный псевдоним System::String. |


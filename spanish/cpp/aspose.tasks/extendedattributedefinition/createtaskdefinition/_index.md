---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition método"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\"."
type: docs
weight: 60
url: /es/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Tasks. Se requiere especificar customFieldType, fieldId y alias al llamar a este método.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| customFieldType | El tipo CustomFieldType especificado. |
| fieldId | El ID de campo ExtendedAttributeTask especificado. |
| alias | El alias System::String especificado. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Tasks. Se requiere especificar fieldId y alias al llamar a este método. El tipo de campo se infiere del id del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| fieldId | El ID de campo ExtendedAttributeTask especificado. |
| alias | El alias System::String especificado. |


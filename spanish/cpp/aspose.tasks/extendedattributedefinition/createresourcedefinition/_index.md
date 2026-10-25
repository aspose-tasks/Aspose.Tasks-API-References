---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition método"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como \"None\"."
type: docs
weight: 50
url: /es/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Resource. Se requiere especificar customFieldType, fieldId y alias al llamar a este método.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| customFieldType | El tipo CustomFieldType especificado. |
| fieldId | El ID de campo ExtendedAttributeResource especificado. |
| alias | El alias System::String especificado. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Método de fábrica que crea una definición de atributo extendido simple, que Microsoft Project muestra como "None". Tiene CalculationType igual a Tasks::CalculationType::None y solo puede usarse en Resource. Se requiere especificar fieldId y alias al llamar a este método. El tipo de campo se infiere del field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| fieldId | El ID de campo ExtendedAttributeResource especificado. |
| alias | El alias System::String especificado. |


---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition método"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks for C++"
description: "Método de fábrica que crea una definición de atributo extendido con búsqueda."
type: docs
weight: 40
url: /es/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Tasks. Se requiere especificar customFieldType, fieldId y alias al llamar a este método.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| customFieldType | El tipo CustomFieldType especificado. |
| fieldId | El ID de campo ExtendedAttributeTask especificado. |
| alias | El alias System::String especificado. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Tasks. Se requiere especificar fieldId y alias al llamar a este método. El tipo de campo se infiere del id del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| fieldId | El ID de campo ExtendedAttributeTask especificado. |
| alias | El alias System::String especificado. |


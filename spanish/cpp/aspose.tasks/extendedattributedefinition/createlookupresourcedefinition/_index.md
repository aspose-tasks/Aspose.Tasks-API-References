---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition method"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks for C++"
description: "Método de fábrica que crea una definición de atributo extendido con búsqueda."
type: docs
weight: 30
url: /es/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Resources. Se requiere especificar customFieldType, fieldId y alias al llamar a este método.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| customFieldType | El tipo CustomFieldType especificado. |
| fieldId | El ID de campo ExtendedAttributeResource especificado. |
| alias | El alias System::String especificado. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Método de fábrica que crea una definición de atributo extendido con búsqueda. Tiene CalculationType igual a Tasks::CalculationType::Lookup y solo puede usarse en Resources. Se requiere especificar fieldId y alias al llamar a este método. El tipo de campo se infiere del id del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parámetro | Descripción |
| --- | --- |
| fieldId | El ID de campo ExtendedAttributeResource especificado. |
| alias | El alias System::String especificado. |


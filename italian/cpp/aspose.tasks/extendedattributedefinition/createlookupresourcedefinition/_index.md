---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition metodo"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks per C++"
description: "Metodo di fabbrica che crea una definizione di attributo esteso con lookup."
type: docs
weight: 30
url: /it/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Resources. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| customFieldType | Il tipo CustomFieldType specificato. |
| fieldId | L'ID campo ExtendedAttributeResource specificato. |
| alias | L'alias System::String specificato. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Metodo factory che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Resources. È necessario specificare fieldId e alias quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| fieldId | L'ID campo ExtendedAttributeResource specificato. |
| alias | L'alias System::String specificato. |


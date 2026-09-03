---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition metodo"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks per C++"
description: "Metodo di fabbrica che crea una definizione di attributo esteso con lookup."
type: docs
weight: 40
url: /it/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Metodo di fabbrica che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Tasks. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| customFieldType | Il tipo CustomFieldType specificato. |
| fieldId | L'ID del campo ExtendedAttributeTask specificato. |
| alias | L'alias System::String specificato. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Metodo factory che crea una definizione di attributo esteso con lookup. Ha CalculationType uguale a Tasks::CalculationType::Lookup e può essere usato solo in Tasks. È necessario specificare fieldId e alias quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| fieldId | L'ID del campo ExtendedAttributeTask specificato. |
| alias | L'alias System::String specificato. |


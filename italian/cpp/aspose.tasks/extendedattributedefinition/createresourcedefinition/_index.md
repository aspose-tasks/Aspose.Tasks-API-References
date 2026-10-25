---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition metodo"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks per C++"
description: "Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\"."
type: docs
weight: 50
url: /it/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere usato solo in Resource. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| customFieldType | Il tipo CustomFieldType specificato. |
| fieldId | L'ID campo ExtendedAttributeResource specificato. |
| alias | L'alias System::String specificato. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Metodo di fabbrica che crea una semplice definizione di attributo esteso, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere utilizzato solo in Resource. È necessario specificare fieldId e alias quando si chiama questo metodo. Il tipo di campo è dedotto dal field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| fieldId | L'ID campo ExtendedAttributeResource specificato. |
| alias | L'alias System::String specificato. |


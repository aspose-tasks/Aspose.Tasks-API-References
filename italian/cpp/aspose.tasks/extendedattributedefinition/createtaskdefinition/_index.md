---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition metodo"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks per C++"
description: "Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come \"None\"."
type: docs
weight: 60
url: /it/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Metodo di fabbrica che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere usato solo in Tasks. È necessario specificare customFieldType, fieldId e alias quando si chiama questo metodo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| customFieldType | Il tipo CustomFieldType specificato. |
| fieldId | L'ID del campo ExtendedAttributeTask specificato. |
| alias | L'alias System::String specificato. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Metodo factory che crea una definizione di attributo esteso semplice, che Microsoft Project mostra come "None". Ha CalculationType uguale a Tasks::CalculationType::None e può essere usato solo in Tasks. È necessario specificare fieldId e alias quando si chiama questo metodo. Il tipo di campo è dedotto dall'ID del campo.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Parametro | Descrizione |
| --- | --- |
| fieldId | L'ID del campo ExtendedAttributeTask specificato. |
| alias | L'alias System::String specificato. |


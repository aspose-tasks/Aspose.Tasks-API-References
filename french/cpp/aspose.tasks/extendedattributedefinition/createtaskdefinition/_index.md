---
title: "Méthode Aspose::Tasks::ExtendedAttributeDefinition::CreateTaskDefinition"
linktitle: "CreateTaskDefinition"
articleTitle: "CreateTaskDefinition"
second_title: "Aspose.Tasks pour C++"
description: "Méthode de fabrique qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\"."
type: docs
weight: 60
url: /fr/cpp/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---

## CreateTaskDefinition (1 of 2) {#createtaskdefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans Tasks. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| customFieldType | Le type CustomFieldType spécifié. |
| fieldId | L'ID de champ ExtendedAttributeTask spécifié. |
| alias | L'alias System::String spécifié. |

---

## CreateTaskDefinition (2 of 2) {#createtaskdefinition_2}

Méthode de fabrique qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans Tasks. Vous devez spécifier fieldId et alias lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| fieldId | L'ID de champ ExtendedAttributeTask spécifié. |
| alias | L'alias System::String spécifié. |


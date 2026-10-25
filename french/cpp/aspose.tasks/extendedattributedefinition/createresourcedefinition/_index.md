---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateResourceDefinition méthode"
linktitle: "CreateResourceDefinition"
articleTitle: "CreateResourceDefinition"
second_title: "Aspose.Tasks pour C++"
description: "Méthode de fabrique qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme \"None\"."
type: docs
weight: 50
url: /fr/cpp/aspose.tasks/extendedattributedefinition/createresourcedefinition/
---

## CreateResourceDefinition (1 of 2) {#createresourcedefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans Resource. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| customFieldType | Le type CustomFieldType spécifié. |
| fieldId | L'ID de champ ExtendedAttributeResource spécifié. |
| alias | L'alias System::String spécifié. |

---

## CreateResourceDefinition (2 of 2) {#createresourcedefinition_2}

Méthode de fabrique qui crée une définition d'attribut étendu simple, que Microsoft Project affiche comme "None". Elle a un CalculationType égal à Tasks::CalculationType::None et ne peut être utilisée que dans les ressources. Vous devez spécifier fieldId et alias lors de l'appel de cette méthode. Le type de champ est déduit de field id.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| fieldId | L'ID de champ ExtendedAttributeResource spécifié. |
| alias | L'alias System::String spécifié. |


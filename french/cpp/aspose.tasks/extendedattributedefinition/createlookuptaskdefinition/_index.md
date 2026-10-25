---
title: "Méthode Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupTaskDefinition"
linktitle: "CreateLookupTaskDefinition"
articleTitle: "CreateLookupTaskDefinition"
second_title: "Aspose.Tasks pour C++"
description: "Méthode de fabrique qui crée une définition d'attribut étendu avec recherche."
type: docs
weight: 40
url: /fr/cpp/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---

## CreateLookupTaskDefinition (1 of 2) {#createlookuptaskdefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Tasks. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupTaskDefinition(CustomFieldType customFieldType, ExtendedAttributeTask fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| customFieldType | Le type CustomFieldType spécifié. |
| fieldId | L'ID de champ ExtendedAttributeTask spécifié. |
| alias | L'alias System::String spécifié. |

---

## CreateLookupTaskDefinition (2 of 2) {#createlookuptaskdefinition_2}

Méthode de fabrique qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Tasks. Vous devez spécifier fieldId et alias lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| fieldId | L'ID de champ ExtendedAttributeTask spécifié. |
| alias | L'alias System::String spécifié. |


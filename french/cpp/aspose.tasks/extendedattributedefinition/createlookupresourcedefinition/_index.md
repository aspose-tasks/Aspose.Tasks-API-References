---
title: "Aspose::Tasks::ExtendedAttributeDefinition::CreateLookupResourceDefinition méthode"
linktitle: "CreateLookupResourceDefinition"
articleTitle: "CreateLookupResourceDefinition"
second_title: "Aspose.Tasks pour C++"
description: "Méthode de fabrique qui crée une définition d'attribut étendu avec recherche."
type: docs
weight: 30
url: /fr/cpp/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---

## CreateLookupResourceDefinition (1 of 2) {#createlookupresourcedefinition_1}

Méthode d'usine qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Resources. Vous devez spécifier customFieldType , fieldId et alias lors de l'appel de cette méthode.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified customFieldType , fieldId and alias .

```cpp
CreateLookupResourceDefinition(CustomFieldType customFieldType, ExtendedAttributeResource fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| customFieldType | Le type CustomFieldType spécifié. |
| fieldId | L'ID de champ ExtendedAttributeResource spécifié. |
| alias | L'alias System::String spécifié. |

---

## CreateLookupResourceDefinition (2 of 2) {#createlookupresourcedefinition_2}

Méthode de fabrique qui crée une définition d'attribut étendu avec recherche. Elle a CalculationType égal à Tasks::CalculationType::Lookup et ne peut être utilisée que dans Resources. Vous devez spécifier fieldId et alias lors de l'appel de cette méthode. Le type de champ est déduit de l'ID du champ.

**Returns:** Created instance of the ExtendedAttributeDefinition class with specified fieldId and alias .

```cpp
CreateLookupResourceDefinition(ExtendedAttributeResource fieldId, const System::String & alias)
```

| Paramètre | Description |
| --- | --- |
| fieldId | L'ID de champ ExtendedAttributeResource spécifié. |
| alias | L'alias System::String spécifié. |


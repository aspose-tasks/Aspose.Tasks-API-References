---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ExtendedAttributeDefinition méthode. Méthode dusine qui crée une définition dattribut étendue avec recherche. Elle aCalculationType est égal àLookup et ne peut être utilisé que dans les ressources. Vous devez spécifierfieldId etalias lors de lappel de cette méthode. Le type de champ est déduit de lID de champ.
type: docs
weight: 10
url: /fr/net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](../calculationtype/) est égal àLookup et ne peut être utilisé que dans les ressources. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | Le spécifié[`ExtendedAttributeResource`](../../extendedattributeresource/) ID de champ. |
| alias | String | Le spécifiéString alias. |

### Return_Value

Instance créée du[`ExtendedAttributeDefinition`](../) classe avec spécifié*fieldId* et*alias*.

### Exemples

Utilisez cet exemple pour créer une définition de champ personnalisé pour une ressource avec recherche, puis remplissez-la avec des valeurs de texte :

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Voir également

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espace de noms [Aspose.Tasks](../../extendedattributedefinition/)
* Assemblée [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](../calculationtype/) est égal àLookup et ne peut être utilisé que dans les ressources. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| customFieldType | CustomFieldType | Le spécifié[`CustomFieldType`](../../customfieldtype/) taper. |
| fieldId | ExtendedAttributeResource | Le spécifié[`ExtendedAttributeResource`](../../extendedattributeresource/) ID de champ. |
| alias | String | Le spécifiéString alias. |

### Return_Value

Instance créée du[`ExtendedAttributeDefinition`](../) classe avec spécifié*customFieldType* ,*fieldId* et*alias*.

### Exemples

Utilisez cet exemple pour créer une définition de champ personnalisé pour une ressource avec recherche, puis remplissez-la avec des valeurs de texte :

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

### Voir également

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* espace de noms [Aspose.Tasks](../../extendedattributedefinition/)
* Assemblée [Aspose.Tasks](../../../)



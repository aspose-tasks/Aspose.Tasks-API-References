---
title: ExtendedAttributeDefinition.CreateLookupTaskDefinition
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ExtendedAttributeDefinition méthode. Méthode dusine qui crée une définition dattribut étendue avec recherche. Elle aCalculationType est égal àLookup et ne peut être utilisé que dans les tâches. Vous devez spécifierfieldId etalias lors de lappel de cette méthode. Le type de champ est déduit de lID de champ.
type: docs
weight: 20
url: /fr/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](../calculationtype/) est égal àLookup et ne peut être utilisé que dans les tâches. Vous devez spécifier*fieldId* et*alias* lors de l'appel de cette méthode. Le type de champ est déduit de l'ID de champ.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Le spécifié[`ExtendedAttributeTask`](../../extendedattributetask/) ID de champ. |
| alias | String | Le spécifiéString alias. |

### Return_Value

Instance créée du[`ExtendedAttributeDefinition`](../) classe avec spécifié*fieldId* et*alias*.

### Exemples

Utilisez cet exemple pour créer une définition de champ personnalisé pour une tâche avec recherche, puis remplissez-la avec des valeurs de texte :

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Voir également

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* espace de noms [Aspose.Tasks](../../extendedattributedefinition/)
* Assemblée [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Méthode d'usine qui crée une définition d'attribut étendue avec recherche. Elle a[`CalculationType`](../calculationtype/) est égal àLookup et ne peut être utilisé que dans les tâches. Vous devez spécifier*customFieldType* ,*fieldId* et*alias* lors de l'appel de cette méthode.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| customFieldType | CustomFieldType | Le spécifié[`CustomFieldType`](../../customfieldtype/) taper. |
| fieldId | ExtendedAttributeTask | Le spécifié[`ExtendedAttributeTask`](../../extendedattributetask/) ID de champ. |
| alias | String | Le spécifiéString alias. |

### Return_Value

Instance créée du[`ExtendedAttributeDefinition`](../) classe avec spécifié*customFieldType* ,*fieldId* et*alias*.

### Exemples

Utilisez cet exemple pour créer une définition de champ personnalisé pour une tâche avec recherche, puis remplissez-la avec des valeurs de texte :

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

### Voir également

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* espace de noms [Aspose.Tasks](../../extendedattributedefinition/)
* Assemblée [Aspose.Tasks](../../../)



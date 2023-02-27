---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Référence de l'API Aspose.Tasks pour .NET
description: ExtendedAttributeDefinition méthode. Ajoute une valeur à la liste de recherche interne. Cest un moyen préférable pour les manipulations avec leValueList .
type: docs
weight: 290
url: /fr/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Ajoute une valeur à la liste de recherche interne. C'est un moyen préférable pour les manipulations avec le[`ValueList`](../valuelist/) .

```csharp
public void AddLookupValue(Value value)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| value | Value | Valeur à ajouter dans la recherche. |

### Remarques

Cette méthode ne fonctionne que pour[`ExtendedAttributeDefinition`](../) instances qui ont[`CalculationType`](../calculationtype/) est égal àLookup .

### Exemples

Utilisez ce code pour ajouter une nouvelle valeur à la liste de recherche :

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

### Voir également

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* espace de noms [Aspose.Tasks](../../extendedattributedefinition/)
* Assemblée [Aspose.Tasks](../../../)



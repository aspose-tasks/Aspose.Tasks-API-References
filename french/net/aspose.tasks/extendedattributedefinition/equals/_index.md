---
title: "ExtendedAttributeDefinition.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Retourne un indicateur indiquant si cette instance est égale à l'objet spécifié."
type: docs
weight: 320
url: /fr/net/aspose.tasks/extendedattributedefinition/equals/
---
## ExtendedAttributeDefinition.Equals method

Renvoie un indicateur indiquant si cette instance est égale à l'objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | l'objet spécifié à comparer à cette instance. |

### Valeur de retour

un indicateur indiquant si cette instance est égale à l'objet spécifié.

## Exemples

Montre comment vérifier l'égalité d'une définition d'attribut étendu.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// l'égalité des calendriers est vérifiée par rapport aux identifiants de champ de définition d'attribut.
Console.WriteLine("ExtendedAttribute 1 Field Id: " + attributeDefinition1.FieldId);
Console.WriteLine("ExtendedAttribute 2 Field Id: " + attributeDefinition2.FieldId);
Console.WriteLine("Are extended attributes equal: " + attributeDefinition1.Equals(attributeDefinition2));
```

### Voir aussi

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)



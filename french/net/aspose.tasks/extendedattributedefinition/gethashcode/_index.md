---
title: "ExtendedAttributeDefinition.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttributeDefinition. Retourne un code de hachage pour l'instance de la classe ExtendedAttributeDefinition."
type: docs
weight: 330
url: /fr/net/aspose.tasks/extendedattributedefinition/gethashcode/
---
## ExtendedAttributeDefinition.GetHashCode method

Retourne un code de hachage pour l'instance de la classe [`ExtendedAttributeDefinition`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

un code de hachage pour cet objet.

## Exemples

Montre comment obtenir un code de hachage d'une définition d'attribut étendu.

```csharp
var project = new Project(DataDir + "MultipleOutlineValues2016.mpp");

var attributeDefinition1 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Start3);
var attributeDefinition2 = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Duration2);

// le code de hachage d'une définition d'attribut étendu est égal à un identifiant de champ.
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition1.FieldId, attributeDefinition1.GetHashCode());
Console.WriteLine("Extended Attribute Field Id: {0} Hash Code: {1}", attributeDefinition2.FieldId, attributeDefinition2.GetHashCode());
```

### Voir aussi

* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)



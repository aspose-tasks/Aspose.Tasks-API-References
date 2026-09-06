---
title: "Resource.ExtendedAttributes"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Resource. Obtient les valeurs d'un attribut étendu"
type: docs
weight: 320
url: /fr/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

Obtient les valeurs d'un attribut étendu.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Remarques

Deux éléments de données sont nécessaires - un pointeur vers la table d'attributs étendus qui est spécifié soit par l'ID unique, soit par l'ID de champ, et la valeur qui est spécifiée soit avec la valeur, soit par un pointeur vers la liste de valeurs.

## Exemples

Montre comment ajouter des attributs étendus de ressource.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// Définir un attribut étendu
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// Créer un attribut étendu et définir sa valeur
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// Ajouter une nouvelle ressource et son attribut étendu
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)



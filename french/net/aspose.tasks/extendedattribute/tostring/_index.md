---
title: "ExtendedAttribute.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ExtendedAttribute. Retourne une représentation courte sous forme de chaîne d'un attribut étendu"
type: docs
weight: 110
url: /fr/net/aspose.tasks/extendedattribute/tostring/
---
## ExtendedAttribute.ToString method

Renvoie une représentation courte sous forme de chaîne d'un attribut étendu.

```csharp
public override string ToString()
```

### Valeur de retour

La représentation sous forme de chaîne de l'attribut étendu.

## Exemples

Montre comment lire les attributs étendus.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Lire les attributs étendus pour les tâches
foreach (var task in project.RootTask.Children)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        // lire les informations communes sur l'attribut étendu
        Console.WriteLine("Extended Attribute: " + attribute.ToString());
    }
}
```

### Voir aussi

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)



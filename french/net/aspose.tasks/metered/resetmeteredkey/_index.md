---
title: "Metered.ResetMeteredKey"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Metered. Supprime la licence précédemment configurée"
type: docs
weight: 30
url: /fr/net/aspose.tasks/metered/resetmeteredkey/
---
## Metered.ResetMeteredKey method

Supprime la licence précédemment configurée.

```csharp
public void ResetMeteredKey()
```

## Exemples

Montre comment utiliser le type de licence &lt;see cref=\"Aspose.Tasks.Metered\" /&gt; avec Aspose.Tasks.

```csharp
// Utilisons la licence à comptage (voir https://purchase.aspose.com/faqs/licensing/metered)
// définir la licence à comptage
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// travailler avec le projet...
// ...

// Nous pouvons obtenir les crédits actuels et la consommation d'octets.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // journaliser l'exception
}

// récemment, l'utilisateur peut réinitialiser une licence à comptage et arrêter le comptage des octets
metered.ResetMeteredKey();
```

### Voir aussi

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)



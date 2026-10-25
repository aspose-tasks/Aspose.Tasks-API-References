---
title: "Metered.SetMeteredKey"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Metered. Définit les clés publiques et privées metered"
type: docs
weight: 40
url: /fr/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Définit les clés publiques et privées mesurées.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| publicKey | Chaîne | La clé publique. |
| privateKey | Chaîne | La clé privée. |

## Remarques

Si vous achetez une licence à consommation, cette API doit être appelée au démarrage de l'application, normalement cela suffit. Cependant, si la licence à consommation échoue à télécharger les données de consommation pendant une période de 24 heures, la licence sera mise en statut d'évaluation. Pour éviter ce cas, vous devez vérifier régulièrement le statut de la licence. Si elle est en statut d'évaluation, appelez à nouveau cette API.

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



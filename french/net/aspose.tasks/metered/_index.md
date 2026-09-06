---
title: "Classe Metered"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Metered. Fournit des méthodes pour définir la clé mesurée"
type: docs
weight: 1020
url: /fr/net/aspose.tasks/metered/
---
## Metered class

Fournit des méthodes pour définir la clé mesurée.

```csharp
public class Metered
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Metered](metered/)() | Le constructeur par défaut. |

## Méthodes

| Nom | Description |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Vérifie si le produit est correctement licencié à l'aide d'une licence Metered. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Supprime la licence précédemment configurée. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Définit les clés publiques et privées mesurées. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Obtient le crédit de consommation. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Obtient la taille du fichier de consommation. |

## Exemples

Dans cet exemple, une tentative sera faite pour définir la clé publique et privée mesurée

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

le fichier jar du composant:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



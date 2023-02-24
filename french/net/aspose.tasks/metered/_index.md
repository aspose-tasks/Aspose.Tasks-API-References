---
title: Class Metered
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.Metered classe. Fournit des méthodes pour définir la clé mesurée.
type: docs
weight: 890
url: /fr/net/aspose.tasks/metered/
---
## Metered class

Fournit des méthodes pour définir la clé mesurée.

```csharp
public class Metered
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [Metered](metered/)() | Default_Constructor |

## Méthodes

| Nom | La description |
| --- | --- |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Supprime la licence précédemment configurée. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Définit des clés publiques et privées mesurées. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Obtient un crédit de consommation. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Obtient la taille du fichier de consommation. |

### Exemples

Dans cet exemple, une tentative sera faite pour définir des clés publiques et privées mesurées

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

le fichier jar du composant :

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)



---
title: Metered.SetMeteredKey
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Metered méthode. Définit des clés publiques et privées mesurées.
type: docs
weight: 30
url: /fr/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Définit des clés publiques et privées mesurées.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| publicKey | String | La clé publique. |
| privateKey | String | La clé privée. |

### Remarques

Si vous achetez une licence mesurée, cette API doit être appelée au démarrage de l'application, normalement, cela suffit. Cependant, si le compteur ne parvient pas à télécharger les données de consommation pendant une période de 24 heures, la licence sera définie sur le statut d'évaluation. Pour éviter ce cas, vous devez vérifier régulièrement l'état de la licence. S'il s'agit d'un état d'évaluation, appelez à nouveau cette API.

### Voir également

* class [Metered](../)
* espace de noms [Aspose.Tasks](../../metered/)
* Assemblée [Aspose.Tasks](../../../)



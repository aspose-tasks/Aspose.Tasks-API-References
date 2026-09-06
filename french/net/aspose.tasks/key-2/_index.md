---
title: "Structure KeyTK"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Structure Aspose.Tasks.Key2TK. Représente une clé de propriété d'une classe du type spécifié. Une instance de cette classe est utilisée lors de l'obtention ou de la définition d'une propriété d'un conteneur."
type: docs
weight: 930
url: /fr/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Représente une clé de propriété d’une classe du type spécifié. Une instance de cette classe est utilisée lors de l’obtention ou de la définition d’une propriété d’un conteneur.

```csharp
public struct Key<T, K>
    where K : struct
```

| Paramètre | Description |
| --- | --- |
| T | Le type de la valeur de la propriété. |
| K | Le type de la clé de propriété. |

## Propriétés

| Nom | Description |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Obtient la clé de la propriété. |

## Exemples

Montre comment lire/écrire la propriété Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



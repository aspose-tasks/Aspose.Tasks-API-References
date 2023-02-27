---
title: Interface IAlgorithmT
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.Util.IAlgorithm1T interface. Représente un algorithme pouvant être appliqué à une liste dobjetsT .
type: docs
weight: 2390
url: /fr/net/aspose.tasks.util/ialgorithm-1/
---
## IAlgorithm&lt;T&gt; interface

Représente un algorithme pouvant être appliqué à une liste d'objets*T* .

```csharp
public interface IAlgorithm<in T>
```

| Paramètre | La description |
| --- | --- |
| T | Type d'objet auquel appliquer l'interface de méthode. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Alg](../../aspose.tasks.util/ialgorithm-1/alg/)(T, int) | Traite un objet de la liste. Appelé après[`PreAlg`](./prealg/) ; |
| [PostAlg](../../aspose.tasks.util/ialgorithm-1/postalg/)(T, int) | Appelé après traitement d'un objet. |
| [PreAlg](../../aspose.tasks.util/ialgorithm-1/prealg/)(T, int) | Appelé avant le traitement d'un objet. |

### Voir également

* espace de noms [Aspose.Tasks.Util](../../aspose.tasks.util/)
* Assemblée [Aspose.Tasks](../../)



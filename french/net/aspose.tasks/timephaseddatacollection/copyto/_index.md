---
title: TimephasedDataCollection.CopyTo
second_title: Référence de l'API Aspose.Tasks pour .NET
description: TimephasedDataCollection méthode. Copie les éléments duTimephasedDataCollection à unArray  à partir dun certainArray index.
type: docs
weight: 90
url: /fr/net/aspose.tasks/timephaseddatacollection/copyto/
---
## TimephasedDataCollection.CopyTo method

Copie les éléments du[`TimephasedDataCollection`](../) à unArray , à partir d'un certainArray index.

```csharp
public void CopyTo(TimephasedData[] array, int arrayIndex)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| array | TimephasedData[] | Le unidimensionnelArray qui est la destination des éléments copiés à partir de[`TimephasedDataCollection`](../) . LeArray doit avoir une indexation de base zéro. |
| arrayIndex | Int32 | L'indice de base zéro dans*array* à laquelle la copie commence. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *array* est nul. |
| ArgumentOutOfRangeException | *arrayIndex* est inférieur à 0. |
| ArgumentException | Le nombre d'éléments dans la source[`TimephasedDataCollection`](../) est supérieur à l'espace disponible à partir de*arrayIndex* jusqu'au bout de la destination*array* . |

### Voir également

* class [TimephasedData](../../timephaseddata/)
* class [TimephasedDataCollection](../)
* espace de noms [Aspose.Tasks](../../timephaseddatacollection/)
* Assemblée [Aspose.Tasks](../../../)



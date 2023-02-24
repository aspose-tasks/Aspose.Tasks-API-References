---
title: TimephasedDataCollection.SelectBetweenStartAndFinish
second_title: Référence de l'API Aspose.Tasks pour .NET
description: TimephasedDataCollection méthode. Sélectionne toutes les phases de temps entrestartTime etfinishTime . A une complexité O log n dans le cas moyen.
type: docs
weight: 120
url: /fr/net/aspose.tasks/timephaseddatacollection/selectbetweenstartandfinish/
---
## TimephasedDataCollection.SelectBetweenStartAndFinish method

Sélectionne toutes les phases de temps entre*startTime* et*finishTime* . A une complexité O (log n) dans le cas moyen.

```csharp
public IList<TimephasedData> SelectBetweenStartAndFinish(TimephasedDataType timephasedDataType, 
    DateTime startTime, DateTime finishTime)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| timephasedDataType | TimephasedDataType | Type de plages horaires à sélectionner. |
| startTime | DateTime | Début de l'intervalle. |
| finishTime | DateTime | Fin de l'intervalle. |

### Return_Value

Renvoie la nouvelle instance de liste de[`TimephasedDataCollection`](../) données triées par la propriété Start.

### Voir également

* class [TimephasedData](../../timephaseddata/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedDataCollection](../)
* espace de noms [Aspose.Tasks](../../timephaseddatacollection/)
* Assemblée [Aspose.Tasks](../../../)



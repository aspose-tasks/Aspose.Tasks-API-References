---
title: TimephasedData.CreateUnitTimephased
second_title: Référence de l'API Aspose.Tasks pour .NET
description: TimephasedData méthode. Crée et initialise une nouvelle instance duTimephasedData classe pour les données échelonnées dans le temps basées sur lunité dune affectation dune ressource matérielle.
type: docs
weight: 30
url: /fr/net/aspose.tasks/timephaseddata/createunittimephased/
---
## TimephasedData.CreateUnitTimephased method

Crée et initialise une nouvelle instance du[`TimephasedData`](../) classe pour les données échelonnées dans le temps basées sur l'unité d'une affectation d'une ressource matérielle.

```csharp
public static TimephasedData CreateUnitTimephased(int uid, DateTime start, DateTime finish, 
    double units, TimephasedDataType type)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| uid | Int32 | UID de la tâche. |
| start | DateTime | Date-heure de début. |
| finish | DateTime | Date-heure de fin. |
| units | Double | Nombre d'unités. |
| type | TimephasedDataType | Type de données chronologiques. |

### Return_Value

Un exemple de[`TimephasedData`](../) classe pour les données chronologiques basées sur les coûts.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Si un nombre négatif d'unités a été spécifié. |

### Voir également

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [TimephasedData](../)
* espace de noms [Aspose.Tasks](../../timephaseddata/)
* Assemblée [Aspose.Tasks](../../../)



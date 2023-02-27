---
title: TaskLink.LinkLagTimeSpan
second_title: Référence de l'API Aspose.Tasks pour .NET
description: TaskLink propriété. Obtient ou définit la durée du décalage en fonction de LagFormat.
type: docs
weight: 50
url: /fr/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Obtient ou définit la durée du décalage, en fonction de LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lorsque vous essayez de définir la valeur pour TaskLinks où LagFormat est TimeUnitType.Percent. |

### Remarques

Le décalage de lien peut être une valeur en pourcentage (LagFormat est TimeUnitType.Percent). Dans ce cas, la durée est calculée en pourcentage de la durée de PredTask. Sinon, la méthode renvoie la valeur TimeSpan représentant le décalage de TaskLink.

### Voir également

* class [TaskLink](../)
* espace de noms [Aspose.Tasks](../../tasklink/)
* Assemblée [Aspose.Tasks](../../../)



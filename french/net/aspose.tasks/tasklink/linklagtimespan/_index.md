---
title: "TaskLink.LinkLagTimeSpan"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLink. Obtient ou définit la durée du retard en fonction de LagFormat"
type: docs
weight: 50
url: /fr/net/aspose.tasks/tasklink/linklagtimespan/
---
## TaskLink.LinkLagTimeSpan property

Obtient ou définit la durée du retard, selon le LagFormat.

```csharp
public TimeSpan LinkLagTimeSpan { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Lors de la tentative de définition de la valeur pour les TaskLinks où LagFormat est TimeUnitType.Percent. |

## Remarques

Le retard de lien peut être une valeur en pourcentage (LagFormat est TimeUnitType.Percent). Dans ce cas, la durée est calculée comme un pourcentage de la durée de PredTask. Sinon, la méthode renvoie une valeur TimeSpan représentant le retard du TaskLink.

### Voir aussi

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)



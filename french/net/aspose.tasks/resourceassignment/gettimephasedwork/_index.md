---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Obtient la quantité de travail phasé dans le temps pour l'intervalle de date et d'heure spécifié"
type: docs
weight: 730
url: /fr/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

Obtient la quantité de travail phasé dans le temps pour l'intervalle de date et d'heure spécifié.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Début de l'intervalle de date et d'heure. |
| fin | DateTime | Fin de l'intervalle de date et d'heure. |
| timephasedDataType | TimephasedDataType | Type des données phasées dans le temps à utiliser. |

## Exemples

Montre comment calculer le travail d'une affectation pour un intervalle de date et d'heure arbitraire.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// Imprimer le travail de l'affectation pour chaque heure.
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### Voir aussi

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

Obtient la quantité de travail phasé dans le temps pour l'intervalle de date et d'heure spécifié.

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | Début de l'intervalle de date et d'heure. |
| fin | DateTime | Fin de l'intervalle de date et d'heure. |

### Voir aussi

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)



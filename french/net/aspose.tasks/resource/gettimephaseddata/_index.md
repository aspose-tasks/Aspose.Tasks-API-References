---
title: "Resource.GetTimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Resource. Retourne une instance de la classe TimephasedDataCollection pour cet objet avec les valeurs TimephasedData comprises entre les dates de début et de fin spécifiées du TimephasedDataType spécifié."
type: docs
weight: 850
url: /fr/net/aspose.tasks/resource/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourne une instance de la classe [`TimephasedDataCollection`](../../timephaseddatacollection/) pour cet objet avec les valeurs [`TimephasedData`](../timephaseddata/) comprises entre les dates de début et de fin spécifiées du [`TimephasedDataType`](../../timephaseddatatype/).

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end, 
    TimephasedDataType timephasedType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début pour les données à phase temporelle. |
| fin | DateTime | La date de fin pour les données à phase temporelle. |
| timephasedType | TimephasedDataType | Le type de données à phase temporelle ([`TimephasedDataType`](../../timephaseddatatype/)). |

### Valeur de retour

Liste de [`TimephasedData`](../timephaseddata/).

## Exemples

Montre comment lire les données à phase temporelle des ressources de travail/coût.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Récupérez la Resource par son ID
var resource = project.Resources.GetByUid(1);

// Imprimez les données à phase temporelle de ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Imprimez les données à phase temporelle de ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourne [`TimephasedDataCollection`](../../timephaseddatacollection/) pour cet objet avec les valeurs [`TimephasedData`](../timephaseddata/) comprises entre les dates de début et de fin spécifiées.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début pour les données à phase temporelle. |
| fin | DateTime | La date de fin pour les données à phase temporelle. |

### Valeur de retour

Liste de [`TimephasedData`](../../timephaseddata/).

## Exemples

Montre comment lire les données à phase temporelle des ressources de travail/coût.

```csharp
var project = new Project(DataDir + "ResourceTimephasedData.mpp");

// Récupérez la Resource par son ID
var resource = project.Resources.GetByUid(1);

// Imprimez les données à phase temporelle de ResourceWork
Console.WriteLine("Timephased data of ResourceWork");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Work: " + td.Value);
}

// Imprimez les données à phase temporelle de ResourceCost
Console.WriteLine("Timephased data of ResourceCost");
foreach (var td in resource.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate), TimephasedDataType.ResourceCost))
{
    Console.Write("Start: " + td.Start.ToShortDateString());
    Console.WriteLine(" Cost: " + td.Value);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)



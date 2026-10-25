---
title: "Task.GetTimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Task. Retourne un objet TimephasedDataCollection contenant des valeurs TimephasedData entre les dates de début et de fin spécifiées du type de données temporelles indiqué."
type: docs
weight: 1360
url: /fr/net/aspose.tasks/task/gettimephaseddata/
---
## GetTimephasedData(DateTime, DateTime, TimephasedDataType) {#gettimephaseddata_1}

Retourne l'objet [`TimephasedDataCollection`](../../timephaseddatacollection/) avec les valeurs [`TimephasedData`](../timephaseddata/) entre les dates de début et de fin données du type de données temporelles spécifié.

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

Un objet [`TimephasedDataCollection`](../../timephaseddatacollection/) contenant des valeurs [`TimephasedData`](../timephaseddata/) entre les dates de début et de fin données du type de données temporelles spécifié.

## Exemples

Montre comment obtenir les données temporelles (avec un type spécifique) de la tâche.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate).AddDays(2), TimephasedDataType.TaskBaselineWork)
    .ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* enum [TimephasedDataType](../../timephaseddatatype/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedData(DateTime, DateTime) {#gettimephaseddata}

Retourne l'objet [`TimephasedDataCollection`](../../timephaseddatacollection/) avec les valeurs [`TimephasedData`](../timephaseddata/) entre les dates de début et de fin données.

```csharp
public TimephasedDataCollection GetTimephasedData(DateTime start, DateTime end)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| début | DateTime | La date de début pour les données à phase temporelle. |
| fin | DateTime | La date de fin pour les données à phase temporelle. |

### Valeur de retour

Liste de [`TimephasedData`](../../timephaseddata/) à remplir.

## Exemples

Montre comment obtenir les données temporelles (avec le type TaskWork) de la tâche.

```csharp
var task = project.RootTask.Children.GetById(1);

List<TimephasedData> data = task.GetTimephasedData(project.Get(Prj.StartDate), project.Get(Prj.FinishDate)).ToList();
foreach (var td in data)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



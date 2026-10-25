---
title: "Task.MoveToSibling"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-methode. Verplaatst de huidige taak op hetzelfde Outline-niveau vóór de opgegeven taak. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate aanroepen na het gebruik van deze methode. Het zal de start/einddatums van alle projecttaken opnieuw plannen, vroege/late datums instellen en de afhankelijke velden zoals slack, werk en kostengebieden en outline-niveaus berekenen. Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak‑id, outline‑niveau en outline‑nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle projecttaken automatisch opnieuw, start/einddatums, stelt vroege/late datums in, berekent slack, werk en kostengebieden, en herberekent id’s en outline‑niveaus"
type: docs
weight: 1370
url: /nl/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Verplaatst de huidige taak op hetzelfde Outline Level vóór de opgegeven taak. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (deze zal alle projecttaken opnieuw plannen (start/finish datums, stelt early/late datums in) en de afhankelijke velden berekenen, zoals slacks, work en cost velden, outline levels). Als ParentProject.CalculationMode Manual is, berekent de methode alleen task id, outline level en outline numbers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle projecttaken automatisch opnieuw (start/finish datums, stelt early/late datums in, berekent slacks, work en cost velden, recalculates ids en outline levels).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beforeTask | Taak | Task vóór welke de huidige taak wordt ingevoegd. |

## Voorbeelden

Toont hoe de taak onder dezelfde ouder te verplaatsen.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Verplaats taken met id 5 vóór taak met id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// OF
// Verplaats taak naar het einde van de collectie
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Verplaatst de huidige taak op hetzelfde Outline Level vóór een taak met de opgegeven Id. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (deze zal alle projecttaken opnieuw plannen (start/finish datums, stelt early/late datums in) en de afhankelijke velden berekenen, zoals slacks, work en cost velden, outline levels). Als ParentProject.CalculationMode Manual is, berekent de methode alleen task id, outline level en outline numbers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle projecttaken automatisch opnieuw (start/finish datums, stelt early/late datums in, berekent slacks, work en cost velden, recalculates ids en outline levels).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) van een taak vóór welke de huidige taak wordt ingevoegd. |

## Voorbeelden

Toont hoe de taak onder dezelfde ouder te verplaatsen met behulp van de Id van de taak.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Verplaats taken met id 5 vóór taak met id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// OF
// Verplaats taak naar het einde van de collectie
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)



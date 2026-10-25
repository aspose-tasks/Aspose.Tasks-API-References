---
title: "Duration.Subtract"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Trekt de opgegeven duur af van deze duurinstantie."
type: docs
weight: 100
url: /nl/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Trekt de opgegeven duur af van deze duur‑instantie.

```csharp
public Duration Subtract(Duration d)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| d | Duration | de opgegeven [`Duration`](../) instantie om van deze instantie af te trekken. |

### Retourwaarde

Nieuw duurobject dat de waarde van deze instantie vertegenwoordigt, min de opgegeven duurwaarde.

## Voorbeelden

Toont hoe je een duur van taken kunt wijzigen.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// een taak ophalen
var task1 = project.RootTask.Children.GetById(1);

// werk de taakduur bij
var duration1 = task1.Get(Tsk.Duration);

// trek één dag af van taak 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// stel een nieuwe duur in voor de taak
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// haal een andere taak op
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// wijzig de duur door het daadwerkelijke tijdseenheidtype te gebruiken
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// stel een nieuwe duur in voor de taak
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Trekt de opgegeven double‑waarde af van deze duur‑instantie.

```csharp
public Duration Subtract(double val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Double | opgegeven Double-waarde om van deze instantie af te trekken. |

### Retourwaarde

Nieuw duurobject dat de waarde van deze instantie vertegenwoordigt, min de opgegeven duurwaarde.

## Voorbeelden

Toont hoe je een duur van taken kunt wijzigen.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// een taak ophalen
var task1 = project.RootTask.Children.GetById(1);

// werk de taakduur bij
var duration1 = task1.Get(Tsk.Duration);

// trek één dag af van taak 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// stel een nieuwe duur in voor de taak
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// haal een andere taak op
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// wijzig de duur door het daadwerkelijke tijdseenheidtype te gebruiken
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// stel een nieuwe duur in voor de taak
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)



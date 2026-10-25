---
title: "Duration.Add"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Duration-methode. Voegt de opgegeven duur toe aan deze duur."
type: docs
weight: 60
url: /nl/net/aspose.tasks/duration/add/
---
## Add(Duration) {#add}

Voegt de opgegeven duur toe aan deze duur.

```csharp
public Duration Add(Duration d)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| d | Duration | opgegeven [`Duration`](../) om toe te voegen aan deze instantie. |

### Retourwaarde

Nieuw duurobject dat de waarde van deze instantie plus de opgegeven duurwaarde vertegenwoordigt.

## Voorbeelden

Toont hoe de duur van taken kan worden bijgewerkt.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// een taak ophalen
var task1 = project.RootTask.Children.GetById(1);

// werk de taakduur bij
var duration1 = task1.Get(Tsk.Duration);

// voeg één dag toe aan taak 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// stel een nieuwe duur in voor de taak
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// haal een andere taak op
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// wijzig de duur door het daadwerkelijke tijdseenheidtype te gebruiken
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// stel een nieuwe duur in voor de taak
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Add(double) {#add_1}

Voegt de opgegeven double‑waarde toe aan deze duur.

```csharp
public Duration Add(double val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Double | de opgegeven Double-waarde om toe te voegen aan deze instantie. |

### Retourwaarde

Nieuw duurobject dat de waarde van deze instantie plus de opgegeven duurwaarde vertegenwoordigt.

## Voorbeelden

Toont hoe de duur van taken kan worden bijgewerkt.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// een taak ophalen
var task1 = project.RootTask.Children.GetById(1);

// werk de taakduur bij
var duration1 = task1.Get(Tsk.Duration);

// voeg één dag toe aan taak 1
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// stel een nieuwe duur in voor de taak
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// haal een andere taak op
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// wijzig de duur door het daadwerkelijke tijdseenheidtype te gebruiken
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// stel een nieuwe duur in voor de taak
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### Zie ook

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)



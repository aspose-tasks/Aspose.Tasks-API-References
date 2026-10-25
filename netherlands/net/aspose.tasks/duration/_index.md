---
title: "Struct Duration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Duration struct. Vertegenwoordigt de duur in een project"
type: docs
weight: 470
url: /nl/net/aspose.tasks/duration/
---
## Duration structure

Stelt de duur in een project voor.

```csharp
public struct Duration : IEquatable<Duration>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | Haalt een waarde op die aangeeft of de tijdseenheid verstreken is. De vlag die bepaalt of deze Duration‑instantie verstreken is. |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | Haalt een waarde op die aangeeft of de tijdseenheid geschat is. De vlag die bepaalt of deze Duration‑instantie geschat is. |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | Haalt de [`TimeSpan`](./timespan/) instantie van dit Duration-object op. De TimeSpan‑instantie van dit Duration-object. |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | Haalt het tijdseenheidtype voor dit object op. Het tijdseenheidtype van deze Duration‑instantie. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | Converteert de opgegeven tekenreeks naar de instantie van de `Duration`‑struct. |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | Voegt de opgegeven double‑waarde toe aan deze duur. |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | Voegt de opgegeven duur toe aan deze duur. |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | Converteert het Duration‑object naar een andere duur met opgegeven tijdseenheden. |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | Retourneert een hashcode‑waarde voor dit object. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | Trekt de opgegeven double‑waarde af van deze duur‑instantie. |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | Trekt de opgegeven duur af van deze duur‑instantie. |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | Converteert het Duration‑object naar een Double‑waarde. |
| override [ToString](../../aspose.tasks/duration/tostring/)() | Retourneert een tekenreeksrepresentatie van deze instantie. |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | Parseert een duurtekenreeks in het formaat "PT--H--M--S--". |
| [operator ==](../../aspose.tasks/duration/op_equality/) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)



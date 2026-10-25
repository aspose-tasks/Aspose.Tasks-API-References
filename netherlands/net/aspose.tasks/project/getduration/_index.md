---
title: "Project.GetDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project‑methode. Haalt een Duration‑object op met het opgegeven aantal eenheden en het standaardduurformaat dat is gedefinieerd in de projectinstellingen DurationFormat."
type: docs
weight: 1100
url: /nl/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Haalt een [`Duration`](../../duration/)‑object op met het opgegeven aantal eenheden en het standaardduurformaat dat is gedefinieerd in de projectinstellingen [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Double | opgegeven aantal eenheden. |

### Retourwaarde

Duration-object.

## Opmerkingen

Deze methode moet zorgvuldig worden gebruikt omdat deze verschillende duurwaarden retourneert, afhankelijk van de instelling Project.DurationFormat. Bijvoorbeeld, GetWork(1.0) retourneert 1 uur wanneer Project.DurationFormat TimeUnitType.Hour is, of 1 dag als Project.DurationFormat TimeUnitType.Day is.

## Voorbeelden

Toont hoe u een &lt;see cref=\"Aspose.Tasks.Duration\" /&gt;‑instantie kunt maken met het standaardduurformaat van het project door project‑fabric‑methoden te gebruiken.

```csharp
var project = new Project();

// haal een duur op met het standaardprojectformaat.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Zie ook

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Haalt een [`Duration`](../../duration/)‑object op met het opgegeven aantal [`TimeUnitType`](../../timeunittype/)‑eenheden.

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Double | opgegeven aantal eenheden. |
| timeUnit | TimeUnitType | opgegeven TimeUnitType‑waarde. |

### Retourwaarde

Duration-object.

## Voorbeelden

Toont hoe u een &lt;see cref=\"Aspose.Tasks.Duration\" /&gt;‑instantie kunt maken door project‑fabric‑methoden te gebruiken.

```csharp
var project = new Project();

// haal een duur op met het standaardprojectformaat.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Zie ook

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Haalt een [`Duration`](../../duration/)‑object op met de opgegeven TimeSpan‑waarde en de opgegeven [`TimeUnitType`](../../timeunittype/)‑waarde.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| timeSpan | TimeSpan | opgegeven TimeSpan‑waarde. |
| timeUnit | TimeUnitType | opgegeven TimeUnitType‑waarde. |

### Retourwaarde

Duration-object.

### Zie ook

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)



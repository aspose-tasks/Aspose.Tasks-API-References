---
title: "Project.Recalculate"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project methode. Plant alle projecttaken opnieuw, ids, outline-niveaus, start-/einddatums, stelt vroege/late datums in, berekent speling, werk- en kostengebieden"
type: docs
weight: 1150
url: /nl/net/aspose.tasks/project/recalculate/
---
## Recalculate() {#recalculate}

Plant alle taak‑ID's, outline‑niveaus, start-/einddatums van het project opnieuw in, stelt vroege/late datums in, berekent speling, werk‑ en kostvelden.

```csharp
public void Recalculate()
```

## Voorbeelden

Toont hoe het project opnieuw te plannen vanaf de startdatum in plaats van de einddatum.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, new DateTime(2014, 1, 1));

// Nu worden alle taakdatums (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) berekend. Om het kritieke pad te verkrijgen moeten we de speling berekenen (kan worden aangeroepen in een aparte thread, maar alleen na de berekening van alle vroege/late datums).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## Recalculate(bool) {#recalculate_1}

Plant alle taak‑ID's, outline‑niveaus, start-/einddatums van het project opnieuw in, stelt vroege/late datums in, berekent speling, werk‑ en kostvelden met optionele validatie.

```csharp
public void Recalculate(bool validate)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| validate | Boolean | Indien true wordt de validatie van de herberekening uitgevoerd. Welke gegevens worden gevalideerd: Op dit moment is alleen basisvalidatie van taak- en taaklink-datumreeksen geïmplementeerd. De datumreeksen van taken (bijv. ActualStart - ActualFinish, EarlyStart - EarlyFinish, enz.) evenals de datums van taaklinks worden gecontroleerd aan de datumcriteria dat de startdatum kleiner of gelijk is aan de einddatum. Als een van de hierboven beschreven voorwaarden niet wordt voldaan, wordt [`RecalculationValidationException`](../../recalculationvalidationexception/) gegooid. |

## Voorbeelden

Toont hoe het project opnieuw te berekenen met postvalidatie.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("t1");
task.Set(Tsk.CommitmentStart, new DateTime(2017, 6, 19, 8, 0, 0));
task.Set(Tsk.CommitmentFinish, new DateTime(2017, 6, 18, 17, 0, 0));

try
{
    // het project opnieuw berekenen met postvalidatie
    project.Recalculate(true);
}
catch (TaskValidationException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Zie ook

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)



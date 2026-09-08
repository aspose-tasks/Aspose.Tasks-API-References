---
title: "Enum ReportType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.ReportType enum. Type van het grafische rapport van het project"
type: docs
weight: 3330
url: /nl/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Type van het grafische rapport van het project.

```csharp
public enum ReportType
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| ProjectOverview | `0` | Toont de start- en einddatum van het project, het percentage van de duur dat voltooid is, het voltooiingspercentage voor taken op het hoogste niveau en aankomende mijlpalen. |
| CostOverview | `1` | Toont de start- en einddatums van het project, de momenteel geplande en resterende kosten, % voltooid en kostwaarden voor taken op het hoogste niveau. |
| WorkOverview | `2` | Toont de basislijn, werkelijke en resterende arbeid voor elke taak op het hoogste niveau en arbeid voor werkresources. |
| ResourceOverview | `3` | Toont de basislijn, werkelijke en resterende arbeid per resource. |
| ResourceCostOverview | `4` | Toont de basislijn, werkelijke en resterende kosten per resource. |
| CriticalTasks | `5` | Toont projecttaken die kritiek zijn. |
| LateTasks | `6` | Toont projecttaken die te laat zijn. |
| Milestones | `7` | Toont mijlpalen die te laat zijn, aankomende en voltooide. |
| UpcomingTask | `8` | Toont taken die deze week moeten worden voltooid en taken die deze week beginnen. |
| CostOverruns | `9` | Toont kostenvariatie per taak en resource. |
| TaskCostOverview | `10` | Toont de basislijn, werkelijke en resterende kosten van alle taken op het hoogste niveau. |
| OverallocatedResources | `11` | Toont het aantal resterende werkuren voor overgealloceerde resources. |
| SlippingTasks | `12` | Toont taken die moeten eindigen na hun basislijn-einddatums (basislijn moet zijn ingesteld). |
| BestPracticeAnalyzer | `13` | Toont taken zonder werkelijke arbeid, niet toegewezen taken, taken met een duur van minder dan 8 uur en samenvattingen toegewezen aan de resources. |
| Burndown | `14` | Bevat werk‑burndown‑ en taak‑burndown‑grafieken. De werk‑burndown‑grafiek toont hoeveel werk mensen hebben voltooid, hoeveel gepland is om te worden voltooid vóór de projecteinddatum, en de basislijnschatting van hoeveel werk op dit moment in het project zou zijn voltooid. De taak‑burndown‑grafiek toont het aantal voltooide taken, het resterende aantal, en de basislijnschatting van hoeveel er op dit moment in het project voltooid zouden zijn. |
| CashFlow | `15` | Toont de kosten en cumulatieve kosten per kwartaal voor alle taken op het hoogste niveau. |

## Voorbeelden

Toont hoe u het project‑burndown‑rapport in PDF‑formaat opslaat naar de opgegeven stream.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



---
title: "Enum ReportType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.ReportType enum. Tipo di report grafico dei progetti"
type: docs
weight: 3330
url: /it/net/aspose.tasks.visualization/reporttype/
---
## ReportType enumeration

Tipo del report grafico del progetto.

```csharp
public enum ReportType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| ProjectOverview | `0` | Mostra la data di inizio e fine del progetto, la percentuale di durata completata, la percentuale completata per le attività di livello superiore e le tappe imminenti. |
| CostOverview | `1` | Mostra le date di inizio e fine del progetto, il costo programmato e residuo attuale, % completato e i valori di costo per le attività di livello superiore. |
| WorkOverview | `2` | Mostra il lavoro di baseline, reale e residuo per ogni attività di livello superiore e il lavoro per le risorse di lavoro. |
| ResourceOverview | `3` | Mostra il lavoro di baseline, reale e residuo per risorsa. |
| ResourceCostOverview | `4` | Mostra il costo di baseline, reale e residuo per risorsa. |
| CriticalTasks | `5` | Mostra le attività del progetto che sono critiche. |
| LateTasks | `6` | Mostra le attività del progetto che sono in ritardo. |
| Milestones | `7` | Mostra le tappe che sono in ritardo, imminenti e completate. |
| UpcomingTask | `8` | Mostra le attività in scadenza durante la settimana corrente e le attività che iniziano durante la settimana corrente. |
| CostOverruns | `9` | Mostra la varianza di costo per attività e per risorsa. |
| TaskCostOverview | `10` | Mostra il costo di baseline, reale e residuo di tutte le attività di livello superiore. |
| OverallocatedResources | `11` | Mostra il numero di ore di lavoro residuo per le risorse sovraassegnate. |
| SlippingTasks | `12` | Mostra le attività che devono terminare dopo le loro date di fine di baseline (la baseline deve essere impostata). |
| BestPracticeAnalyzer | `13` | Mostra le attività senza lavoro reale, le attività non assegnate, le attività con durata inferiore a 8 ore e i riepiloghi assegnati alle risorse. |
| Burndown | `14` | Include i grafici work burndown e task burndown. Il grafico work burndown mostra quanto lavoro le persone hanno completato, quanto è programmato per essere completato prima della data di fine progetto, e la stima di baseline di quanto lavoro sarebbe completato a questo punto del progetto. Il grafico task burndown mostra il numero di attività completate, il numero residuo e la stima di baseline di quante sarebbero completate a questo punto del progetto. |
| CashFlow | `15` | Mostra i costi e i costi cumulativi per trimestre per tutte le attività di livello superiore. |

## Esempi

Mostra come salvare il report di avanzamento del progetto in formato PDF nello stream specificato.

```csharp
var project = new Project(DataDir + @"Homemoveplan.mpp");
using (var stream = new FileStream(OutDir + "Burndown_out.pdf", FileMode.Create))
{
    project.SaveReport(stream, ReportType.Burndown);
}
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)



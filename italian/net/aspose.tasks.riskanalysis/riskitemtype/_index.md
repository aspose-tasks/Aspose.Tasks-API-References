---
title: "Enum RiskItemType"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Enum Aspose.Tasks.RiskAnalysis.RiskItemType. Specifica i campi delle attività per i quali vengono raccolte le informazioni statistiche durante l'analisi del rischio."
type: docs
weight: 1920
url: /it/net/aspose.tasks.riskanalysis/riskitemtype/
---
## RiskItemType enumeration

Specifica i campi delle attività per i quali vengono raccolte le informazioni statistiche durante l'analisi del rischio.

```csharp
public enum RiskItemType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Start | `0` | Inizio attività. |
| Finish | `1` | Fine attività. |
| EarlyStart | `2` | Inizio anticipato attività. |
| EarlyFinish | `3` | Fine anticipata attività. |
| LateStart | `4` | Inizio ritardato attività. |
| LateFinish | `5` | Fine ritardata attività. |

## Esempi

Mostra come calcolare le statistiche dei rischi e salvarle come report PDF.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Inizializza un modello di rischio
var pattern = new RiskPattern(task)
{
    // Seleziona un tipo di distribuzione per il generatore di numeri casuali da cui generare valori possibili (attualmente sono supportati solo due tipi, ovvero normale e uniforme)
    // Per ulteriori dettagli vedi qui: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore
    // Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni
    Optimistic = 70,

    // Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore
    // Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni.
    Pessimistic = 130,

    // Imposta un livello di confidenza che corrisponde alla percentuale di tempo in cui i valori reali saranno compresi tra le stime ottimistiche e pessimistiche.
    // Puoi considerarlo come un valore di deviazione standard: più sei incerto sulle tue stime, più il valore di deviazione standard usato nel generatore di numeri casuali sarà elevato.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Analizza i rischi del progetto
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);

// salva l'analisi come report in un file tramite percorso file
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// oppure salva l'analisi in uno stream
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Vedi anche

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)



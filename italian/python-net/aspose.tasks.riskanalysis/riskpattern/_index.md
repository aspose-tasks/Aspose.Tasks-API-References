---
title: "RiskPattern"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 60
url: /it/python-net/aspose.tasks.riskanalysis/riskpattern/
---

## RiskPattern class

Rappresenta un modello di rischio per un'attività di progetto.

Il tipo RiskPattern espone i seguenti membri:
## Costruttori
| Nome | Descrizione |
| :- | :- |
| RiskPattern(task) | Inizializza una nuova istanza della classe [RiskPattern](/tasks/python-net/aspose.tasks.riskanalysis/riskpattern/). |
## Proprietà
| Nome | Descrizione |
| :- | :- |
| task | Ottiene un'attività di progetto a cui viene applicato questo modello di rischio. |
| distribution | Ottiene o imposta la distribuzione di probabilità utilizzata nella simulazione Monte Carlo.<br/>            Il valore predefinito è ProbabilityDistributionType.Normal. |
| confidence_level | Ottiene o imposta il livello di confidenza che corrisponde alla percentuale di volte in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche.<br/>            Il valore predefinito è CL99. |
| optimistic | Ottiene o imposta la percentuale della durata dell'attività più probabile che può verificarsi nello scenario di progetto migliore possibile.<br/>            Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni. |
| pessimistic | Ottiene o imposta la percentuale della durata dell'attività più probabile che può verificarsi nello scenario di progetto peggiore possibile.<br/>            Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni. |

### Vedi anche

* namespace [aspose.tasks.riskanalysis](/tasks/python-net/aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](/tasks/python-net/)


---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un modello di rischio per un'attività di progetto."
type: docs
weight: 268
url: /it/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Rappresenta un modello di rischio per un'attività di progetto.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Inizializza una nuova istanza della classe [RiskPattern](../../com.aspose/tasks/riskpattern). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Restituisce il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche. |
| [getDistribution()](#getDistribution--) | Restituisce la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. |
| [getOptimistic()](#getOptimistic--) | Restituisce la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile. |
| [getPessimistic()](#getPessimistic--) | Restituisce la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile. |
| [getTask()](#getTask--) | Ottiene un'attività di progetto a cui viene applicato questo modello di rischio. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Imposta il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche. |
| [setDistribution(int value)](#setDistribution-int-) | Imposta la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. |
| [setOptimistic(int value)](#setOptimistic-int-) | Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile. |
| [setPessimistic(int value)](#setPessimistic-int-) | Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Inizializza una nuova istanza della classe [RiskPattern](../../com.aspose/tasks/riskpattern).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | l'attività di progetto specificata per la quale questo rischio sarà applicato nella simulazione Monte Carlo. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Ottiene il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche. Il valore predefinito è CL99.

--------------------

Può essere uno dei valori definiti nell'enumerazione `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Returns:**
int - il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Ottiene la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. Il valore predefinito è ProbabilityDistributionType.Normal.

--------------------

Può essere uno dei valori definiti nell'enumerazione [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Returns:**
int - la distribuzione di probabilità utilizzata nella simulazione Monte Carlo.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Ottiene la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile. Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni.

**Returns:**
int - la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Ottiene la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile. Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni.

**Returns:**
int - la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile.
### getTask() {#getTask--}
```
public final Task getTask()
```


Ottiene un'attività di progetto a cui viene applicato questo modello di rischio.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Imposta il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche. Il valore predefinito è CL99.

--------------------

Può essere uno dei valori definiti nell'enumerazione `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | il livello di confidenza che corrisponde alla percentuale di tempo in cui i valori generati effettivi saranno compresi tra le stime ottimistiche e pessimistiche. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Imposta la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. Il valore predefinito è ProbabilityDistributionType.Normal.

--------------------

Può essere uno dei valori definiti nell'enumerazione [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la distribuzione di probabilità utilizzata nella simulazione Monte Carlo. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile. Il valore predefinito è 75, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata ottimistica sarà 3 giorni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto migliore possibile. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Imposta la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile. Il valore predefinito è 125, il che significa che se la durata stimata dell'attività specificata è 4 giorni, la durata pessimistica sarà 5 giorni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | la percentuale della durata più probabile dell'attività che può verificarsi nello scenario di progetto peggiore possibile. |


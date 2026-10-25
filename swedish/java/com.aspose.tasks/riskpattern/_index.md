---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar ett riskmönster för en projektuppgift."
type: docs
weight: 268
url: /sv/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Representerar ett riskmönster för en projektuppgift.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Initierar en ny instans av klassen [RiskPattern](../../com.aspose.tasks/riskpattern). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Hämtar förtroendenivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar. |
| [getDistribution()](#getDistribution--) | Hämtar sannolikhetsfördelningen som används i Monte Carlo-simulering. |
| [getOptimistic()](#getOptimistic--) | Hämtar procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot. |
| [getPessimistic()](#getPessimistic--) | Hämtar procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot. |
| [getTask()](#getTask--) | Hämtar en projektuppgift som detta riskmönster tillämpas på. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Ställer in förtroendenivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar. |
| [setDistribution(int value)](#setDistribution-int-) | Ställer in sannolikhetsfördelningen som används i Monte Carlo-simulering. |
| [setOptimistic(int value)](#setOptimistic-int-) | Ställer in procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot. |
| [setPessimistic(int value)](#setPessimistic-int-) | Ställer in procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Initierar en ny instans av klassen [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | den specificerade projektuppgiften som detta risk kommer att tillämpas på i Monte Carlo-simulering. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Hämtar förtroendenivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar. Standardvärdet är CL99.

--------------------

Kan vara ett av värdena som definieras i `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-))‑enumerationen.

**Returns:**
int - förtroendenivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Hämtar sannolikhetsfördelningen som används i Monte Carlo-simulering. Standardvärdet är ProbabilityDistributionType.Normal.

--------------------

Kan vara ett av värdena som definieras i [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype)‑enumerationen.

**Returns:**
int - sannolikhetsfördelningen som används i Monte Carlo-simulering.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Hämtar procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot. Standardvärdet är 75, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den optimistiska varaktigheten 3 dagar.

**Returns:**
int - procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Hämtar procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot. Standardvärdet är 125, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den pessimistiska varaktigheten 5 dagar.

**Returns:**
int - procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot.
### getTask() {#getTask--}
```
public final Task getTask()
```


Hämtar en projektuppgift som detta riskmönster tillämpas på.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Ställer in förtroendenivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar. Standardvärdet är CL99.

--------------------

Kan vara ett av värdena som definieras i `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-))‑enumerationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | konfidensnivån som motsvarar den procentandel av tiden som de faktiska genererade värdena kommer att ligga inom optimistiska och pessimistiska uppskattningar. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Ställer in sannolikhetsfördelningen som används i Monte Carlo-simulering. Standardvärdet är ProbabilityDistributionType.Normal.

--------------------

Kan vara ett av värdena som definieras i [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype)‑enumerationen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | sannolikhetsfördelningen som används i Monte Carlo-simulering. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Ställer in procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot. Standardvärdet är 75, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den optimistiska varaktigheten 3 dagar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det bästa möjliga projektscenariot. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Ställer in procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot. Standardvärdet är 125, vilket betyder att om den uppskattade specificerade uppgiftens varaktighet är 4 dagar så blir den pessimistiska varaktigheten 5 dagar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | procentsatsen för den mest sannolika uppgiftens varaktighet som kan inträffa i det sämsta möjliga projektscenariot. |


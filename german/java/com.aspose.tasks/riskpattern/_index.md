---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt ein Risikomuster für eine Projektaufgabe dar."
type: docs
weight: 268
url: /de/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Stellt ein Risikomuster für eine Projektaufgabe dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Initialisiert eine neue Instanz der [RiskPattern](../../com.aspose.tasks/riskpattern) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Ruft den Konfidenzwert ab, der dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb optimistischer und pessimistischer Schätzungen liegen. |
| [getDistribution()](#getDistribution--) | Ruft die in der Monte‑Carlo‑Simulation verwendete Wahrscheinlichkeitsverteilung ab. |
| [getOptimistic()](#getOptimistic--) | Ruft den Prozentsatz der wahrscheinlichsten Aufgabendauer ab, der im bestmöglichen Projektszenario auftreten kann. |
| [getPessimistic()](#getPessimistic--) | Ruft den Prozentsatz der wahrscheinlichsten Aufgabendauer ab, der im ungünstigsten Projektszenario auftreten kann. |
| [getTask()](#getTask--) | Ruft eine Projektaufgabe ab, auf die dieses Risikomuster angewendet wird. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Setzt den Konfidenzwert, der dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb optimistischer und pessimistischer Schätzungen liegen. |
| [setDistribution(int value)](#setDistribution-int-) | Setzt die in der Monte‑Carlo‑Simulation verwendete Wahrscheinlichkeitsverteilung. |
| [setOptimistic(int value)](#setOptimistic-int-) | Setzt den Prozentsatz der wahrscheinlichsten Aufgabendauer, der im bestmöglichen Projektszenario auftreten kann. |
| [setPessimistic(int value)](#setPessimistic-int-) | Setzt den Prozentsatz der wahrscheinlichsten Aufgabendauer, der im ungünstigsten Projektszenario auftreten kann. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Initialisiert eine neue Instanz der [RiskPattern](../../com.aspose.tasks/riskpattern) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | die angegebene Projektaufgabe, für die dieses Risiko in der Monte‑Carlo‑Simulation angewendet wird. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Ruft den Konfidenzwert ab, der dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb optimistischer und pessimistischer Schätzungen liegen. Der Standardwert ist CL99.

--------------------

Kann einer der in der `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) Aufzählung definierten Werte sein.

**Returns:**
int - der Konfidenzwert, der dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb optimistischer und pessimistischer Schätzungen liegen.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Ruft die Wahrscheinlichkeitsverteilung ab, die in der Monte‑Carlo‑Simulation verwendet wird. Der Standardwert ist ProbabilityDistributionType.Normal.

--------------------

Kann einer der in der [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) Aufzählung definierten Werte sein.

**Returns:**
int - die in der Monte‑Carlo‑Simulation verwendete Wahrscheinlichkeitsverteilung.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Ruft den Prozentsatz der wahrscheinlichsten Aufgabendauer ab, der im bestmöglichen Projektszenario auftreten kann. Der Standardwert ist 75, was bedeutet, dass wenn die geschätzte angegebene Aufgabendauer 4 Tage beträgt, die optimistische Dauer 3 Tage beträgt.

**Returns:**
int - der Prozentsatz der wahrscheinlichsten Aufgabendauer, der im bestmöglichen Projektszenario auftreten kann.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Ruft den Prozentsatz der wahrscheinlichsten Aufgabendauer ab, der im ungünstigsten Projektszenario auftreten kann. Der Standardwert ist 125, was bedeutet, dass wenn die geschätzte angegebene Aufgabendauer 4 Tage beträgt, die pessimistische Dauer 5 Tage beträgt.

**Returns:**
int - der Prozentsatz der wahrscheinlichsten Aufgabendauer, der im ungünstigsten Projektszenario auftreten kann.
### getTask() {#getTask--}
```
public final Task getTask()
```


Ruft eine Projektaufgabe ab, auf die dieses Risikomuster angewendet wird.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Legt das Konfidenzniveau fest, das dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb der optimistischen und pessimistischen Schätzungen liegen. Der Standardwert ist CL99.

--------------------

Kann einer der in der `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose.tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose.tasks/riskpattern\#setConfidenceLevel-int-)) Aufzählung definierten Werte sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | das Konfidenzniveau, das dem Prozentsatz der Zeit entspricht, in der die tatsächlich generierten Werte innerhalb der optimistischen und pessimistischen Schätzungen liegen. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Legt die in der Monte‑Carlo‑Simulation verwendete Wahrscheinlichkeitsverteilung fest. Der Standardwert ist ProbabilityDistributionType.Normal.

--------------------

Kann einer der in der [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype) Aufzählung definierten Werte sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | die in der Monte‑Carlo‑Simulation verwendete Wahrscheinlichkeitsverteilung. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Legt den Prozentsatz der wahrscheinlichsten Aufgabendauer fest, der im bestmöglichen Projektszenario auftreten kann. Der Standardwert ist 75, was bedeutet, dass wenn die geschätzte angegebene Aufgabendauer 4 Tage beträgt, die optimistische Dauer 3 Tage beträgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Prozentsatz der wahrscheinlichsten Aufgabendauer, der im bestmöglichen Projektszenario auftreten kann. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Legt den Prozentsatz der wahrscheinlichsten Aufgabendauer fest, der im ungünstigsten Projektszenario auftreten kann. Der Standardwert ist 125, was bedeutet, dass wenn die geschätzte angegebene Aufgabendauer 4 Tage beträgt, die pessimistische Dauer 5 Tage beträgt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | der Prozentsatz der wahrscheinlichsten Aufgabendauer, der im ungünstigsten Projektszenario auftreten kann. |


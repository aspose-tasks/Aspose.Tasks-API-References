---
title: "RiskPattern"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Vertegenwoordigt een risicopatroon voor een projecttaak."
type: docs
weight: 268
url: /nl/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Vertegenwoordigt een risicopatroon voor een projecttaak.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Initialiseert een nieuw exemplaar van de [RiskPattern](../../com.aspose.tasks/riskpattern) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Haalt het vertrouwensniveau op dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen vallen. |
| [getDistribution()](#getDistribution--) | Haalt de kansverdeling op die wordt gebruikt in Monte‑Carlo‑simulatie. |
| [getOptimistic()](#getOptimistic--) | Haalt het percentage op van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario. |
| [getPessimistic()](#getPessimistic--) | Haalt het percentage op van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario. |
| [getTask()](#getTask--) | Haalt een projecttaak op waaraan dit risicopatroon wordt toegepast. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Stelt het betrouwbaarheidsniveau in dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen zullen liggen. |
| [setDistribution(int value)](#setDistribution-int-) | Stelt de kansverdeling in die wordt gebruikt in Monte Carlo-simulatie. |
| [setOptimistic(int value)](#setOptimistic-int-) | Stelt het percentage in van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario. |
| [setPessimistic(int value)](#setPessimistic-int-) | Stelt het percentage in van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Initialiseert een nieuw exemplaar van de [RiskPattern](../../com.aspose.tasks/riskpattern) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | de opgegeven projecttaak waarvoor dit risico wordt toegepast in Monte Carlo-simulatie. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Haalt het betrouwbaarheidsniveau op dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen zullen liggen. De standaardwaarde is CL99.

--------------------

Kan een van de waarden zijn die gedefinieerd zijn in de `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) enumeratie.

**Returns:**
int - het betrouwbaarheidsniveau dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen zullen liggen.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Haalt de kansverdeling op die wordt gebruikt in Monte Carlo-simulatie. De standaardwaarde is ProbabilityDistributionType.Normal.

--------------------

Kan een van de waarden zijn die gedefinieerd zijn in de [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype) enumeratie.

**Returns:**
int - de kansverdeling die wordt gebruikt in Monte Carlo-simulatie.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Haalt het percentage op van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario. De standaardwaarde is 75, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de optimistische duur 3 dagen zal zijn.

**Returns:**
int - het percentage van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Haalt het percentage op van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario. De standaardwaarde is 125, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de pessimistische duur 5 dagen zal zijn.

**Returns:**
int - het percentage van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario.
### getTask() {#getTask--}
```
public final Task getTask()
```


Haalt een projecttaak op waaraan dit risicopatroon wordt toegepast.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Stelt het betrouwbaarheidsniveau in dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen zullen liggen. De standaardwaarde is CL99.

--------------------

Kan een van de waarden zijn die gedefinieerd zijn in de `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)) enumeratie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het betrouwbaarheidsniveau dat overeenkomt met het percentage van de tijd dat de daadwerkelijk gegenereerde waarden binnen optimistische en pessimistische schattingen zullen liggen. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Stelt de kansverdeling in die wordt gebruikt in Monte Carlo-simulatie. De standaardwaarde is ProbabilityDistributionType.Normal.

--------------------

Kan een van de waarden zijn die gedefinieerd zijn in de [ProbabilityDistributionType](../../com.aspose/tasks/probabilitydistributiontype) enumeratie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | de kansverdeling die wordt gebruikt in Monte Carlo-simulatie. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Stelt het percentage in van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario. De standaardwaarde is 75, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de optimistische duur 3 dagen zal zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het percentage van de meest waarschijnlijke taakduur die kan optreden in het best mogelijke projectscenario. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Stelt het percentage in van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario. De standaardwaarde is 125, wat betekent dat als de geschatte opgegeven taakduur 4 dagen is, de pessimistische duur 5 dagen zal zijn.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | het percentage van de meest waarschijnlijke taakduur die kan optreden in het slechtst mogelijke projectscenario. |


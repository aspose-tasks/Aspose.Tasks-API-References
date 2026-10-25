---
title: "RiskPattern"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un modèle de risque pour une tâche de projet."
type: docs
weight: 268
url: /fr/java/com.aspose.tasks/riskpattern/
---

**Inheritance:**
java.lang.Object
```
public class RiskPattern
```

Représente un modèle de risque pour une tâche de projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RiskPattern(Task task)](#RiskPattern-com.aspose.tasks.Task-) | Initialise une nouvelle instance de la classe [RiskPattern](../../com.aspose.tasks/riskpattern). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getConfidenceLevel()](#getConfidenceLevel--) | Obtient le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes. |
| [getDistribution()](#getDistribution--) | Obtient la distribution de probabilité utilisée dans la simulation Monte Carlo. |
| [getOptimistic()](#getOptimistic--) | Obtient le pourcentage de la durée la plus probable d'une tâche qui peut se produire dans le meilleur scénario de projet possible. |
| [getPessimistic()](#getPessimistic--) | Obtient le pourcentage de la durée la plus probable d'une tâche qui peut se produire dans le pire scénario de projet possible. |
| [getTask()](#getTask--) | Obtient une tâche de projet à laquelle ce modèle de risque est appliqué. |
| [setConfidenceLevel(int value)](#setConfidenceLevel-int-) | Définit le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes. |
| [setDistribution(int value)](#setDistribution-int-) | Définit la distribution de probabilité utilisée dans la simulation Monte Carlo. |
| [setOptimistic(int value)](#setOptimistic-int-) | Définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible. |
| [setPessimistic(int value)](#setPessimistic-int-) | Définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible. |
### RiskPattern(Task task) {#RiskPattern-com.aspose.tasks.Task-}
```
public RiskPattern(Task task)
```


Initialise une nouvelle instance de la classe [RiskPattern](../../com.aspose.tasks/riskpattern).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | la tâche de projet spécifiée pour laquelle ce risque sera appliqué dans la simulation Monte Carlo. |

### getConfidenceLevel() {#getConfidenceLevel--}
```
public final int getConfidenceLevel()
```


Obtient le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes. La valeur par défaut est CL99.

--------------------

Peut être l'une des valeurs définies dans l'énumération `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Returns:**
int - le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes.
### getDistribution() {#getDistribution--}
```
public final int getDistribution()
```


Obtient la distribution de probabilité utilisée dans la simulation Monte Carlo. La valeur par défaut est ProbabilityDistributionType.Normal.

--------------------

Peut être l'une des valeurs définies dans l'énumération [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Returns:**
int - la distribution de probabilité utilisée dans la simulation Monte Carlo.
### getOptimistic() {#getOptimistic--}
```
public final int getOptimistic()
```


Obtient le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible. La valeur par défaut est 75, ce qui signifie que si la durée de tâche spécifiée estimée est de 4 jours, alors la durée optimiste sera de 3 jours.

**Returns:**
int - le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible.
### getPessimistic() {#getPessimistic--}
```
public final int getPessimistic()
```


Obtient le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible. La valeur par défaut est 125, ce qui signifie que si la durée de tâche spécifiée estimée est de 4 jours, alors la durée pessimiste sera de 5 jours.

**Returns:**
int - le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible.
### getTask() {#getTask--}
```
public final Task getTask()
```


Obtient une tâche de projet à laquelle ce modèle de risque est appliqué.

**Returns:**
[Task](../../com.aspose.tasks/task) - a project task to which this risk pattern is applied.
### setConfidenceLevel(int value) {#setConfidenceLevel-int-}
```
public final void setConfidenceLevel(int value)
```


Définit le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes. La valeur par défaut est CL99.

--------------------

Peut être l'une des valeurs définies dans l'énumération `ConfidenceLevel`([getConfidenceLevel()](../../com.aspose/tasks/riskpattern\#getConfidenceLevel--)/[setConfidenceLevel(int)](../../com.aspose/tasks/riskpattern\#setConfidenceLevel-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le niveau de confiance qui correspond au pourcentage du temps pendant lequel les valeurs réellement générées seront comprises entre les estimations optimistes et pessimistes. |

### setDistribution(int value) {#setDistribution-int-}
```
public final void setDistribution(int value)
```


Définit la distribution de probabilité utilisée dans la simulation Monte Carlo. La valeur par défaut est ProbabilityDistributionType.Normal.

--------------------

Peut être l'une des valeurs définies dans l'énumération [ProbabilityDistributionType](../../com.aspose.tasks/probabilitydistributiontype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la distribution de probabilité utilisée dans la simulation Monte Carlo. |

### setOptimistic(int value) {#setOptimistic-int-}
```
public final void setOptimistic(int value)
```


Définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible. La valeur par défaut est 75, ce qui signifie que si la durée de tâche spécifiée estimée est de 4 jours, alors la durée optimiste sera de 3 jours.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le pourcentage de la durée de tâche la plus probable qui peut se produire dans le meilleur scénario de projet possible. |

### setPessimistic(int value) {#setPessimistic-int-}
```
public final void setPessimistic(int value)
```


Définit le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible. La valeur par défaut est 125, ce qui signifie que si la durée de tâche spécifiée estimée est de 4 jours, alors la durée pessimiste sera de 5 jours.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le pourcentage de la durée de tâche la plus probable qui peut se produire dans le pire scénario de projet possible. |


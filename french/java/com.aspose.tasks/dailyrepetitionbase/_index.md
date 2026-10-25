---
title: "DailyRepetitionBase"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une classe de base pour les répétitions dans un modèle de récurrence quotidien."
type: docs
weight: 65
url: /fr/java/com.aspose.tasks/dailyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class DailyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Représente une classe de base pour les répétitions dans un modèle de récurrence quotidien.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \{@inheritDoc\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Obtient un nombre de jours qui représente l'intervalle en jours entre les occurrences. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \{@inheritDoc\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Définit un nombre de jours qui représente l'intervalle en jours entre les occurrences. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Obtient un calculateur utilisé pour calculer une répétition.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \{@inheritDoc\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Obtient un nombre de jours qui représente l'intervalle en jours entre les occurrences.

**Returns:**
int - un nombre de jours qui représente l'intervalle en jours entre les occurrences.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Obtient un validateur pour le modèle de récurrence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \{@inheritDoc\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Définit un nombre de jours qui représente l'intervalle en jours entre les occurrences.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de jours qui représente l'intervalle en jours entre les occurrences. |


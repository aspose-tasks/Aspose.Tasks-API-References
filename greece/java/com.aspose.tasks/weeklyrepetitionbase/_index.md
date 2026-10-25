---
title: "WeeklyRepetitionBase"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια βασική κλάση για επαναλήψεις σε εβδομαδιαίο μοτίβο επανάληψης."
type: docs
weight: 358
url: /el/java/com.aspose.tasks/weeklyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class WeeklyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Αναπαριστά μια βασική κλάση για επαναλήψεις σε εβδομαδιαίο μοτίβο επανάληψης.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \\{@inheritDoc\\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Λαμβάνει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \\{@inheritDoc\\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων. |
### getCalculator(Calendar calendar, Duration duration) {#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-}
```
public final RecurrenceDateCalculatorBase getCalculator(Calendar calendar, Duration duration)
```


Λαμβάνει έναν υπολογιστή που χρησιμοποιείται για τον υπολογισμό μιας επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \\{@inheritDoc\\} |
| duration | [Duration](../../com.aspose.tasks/duration) | \\{@inheritDoc\\} |

**Returns:**
com.aspose.tasks.RecurrenceDateCalculatorBase - \\{@inheritDoc\\}
### getRepetitionInterval() {#getRepetitionInterval--}
```
public final int getRepetitionInterval()
```


Λαμβάνει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων.

**Returns:**
int - ένας αριθμός εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων.
### getValidator(Calendar calendar) {#getValidator-com.aspose.tasks.Calendar-}
```
public final RecurrencePatternValidatorBase getValidator(Calendar calendar)
```


Λαμβάνει έναν επικυρωτή για το πρότυπο επανάληψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | \\{@inheritDoc\\} |

**Returns:**
com.aspose.tasks.RecurrencePatternValidatorBase - \\{@inheritDoc\\}
### setRepetitionInterval(int value) {#setRepetitionInterval-int-}
```
public final void setRepetitionInterval(int value)
```


Ορίζει έναν αριθμό εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας αριθμός εβδομάδων που αντιπροσωπεύει το διάστημα σε εβδομάδες μεταξύ των εμφανίσεων. |


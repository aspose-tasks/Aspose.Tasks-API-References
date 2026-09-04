---
title: "MonthlyRepetitionBase"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει ένα βασικό μοτίβο για τη θέση της ημέρας του μήνα."
type: docs
weight: 159
url: /el/java/com.aspose.tasks/monthlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class MonthlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Αντιπροσωπεύει ένα βασικό μοτίβο για τη θέση της ημέρας του μήνα.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \\{@inheritDoc\\} |
| [getRepetitionInterval()](#getRepetitionInterval--) | Λαμβάνει έναν αριθμό μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων. |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \\{@inheritDoc\\} |
| [setRepetitionInterval(int value)](#setRepetitionInterval-int-) | Ορίζει έναν αριθμό μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων. |
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


Λαμβάνει έναν αριθμό μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων.

**Returns:**
int - ένας αριθμός μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων.
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


Ορίζει έναν αριθμό μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας αριθμός μηνών που αντιπροσωπεύει το διάστημα σε μήνες μεταξύ των εμφανίσεων. |


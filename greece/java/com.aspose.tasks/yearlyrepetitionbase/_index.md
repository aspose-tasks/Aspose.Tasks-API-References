---
title: "YearlyRepetitionBase"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ένα βασικό μοτίβο για τη θέση της ετήσιας ημέρας."
type: docs
weight: 372
url: /el/java/com.aspose.tasks/yearlyrepetitionbase/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.IValidatorCreator, com.aspose.tasks.ICalculatorCreator
```
public abstract class YearlyRepetitionBase implements IValidatorCreator, ICalculatorCreator
```

Αναπαριστά ένα βασικό μοτίβο για τη θέση της ετήσιας ημέρας.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCalculator(Calendar calendar, Duration duration)](#getCalculator-com.aspose.tasks.Calendar-com.aspose.tasks.Duration-) | \\{@inheritDoc\\} |
| [getValidator(Calendar calendar)](#getValidator-com.aspose.tasks.Calendar-) | \\{@inheritDoc\\} |
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

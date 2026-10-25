---
title: "ConstraintType"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Καθορίζει τον περιορισμό στην ημερομηνία έναρξης ή λήξης μιας εργασίας."
type: docs
weight: 52
url: /el/java/com.aspose.tasks/constrainttype/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class ConstraintType extends System.Enum
```

Καθορίζει τον περιορισμό στην ημερομηνία έναρξης ή λήξης μιας εργασίας. Κατά την εξαγωγή σε XML οι τιμές Undefined θα αφαιρεθούν από το παραγόμενο XML.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [AsLateAsPossible](#AsLateAsPossible) | `Tsk.Start` και `Tsk.Finish` ημερομηνίες του `Task` προγραμματίζονται ALAP σε σχέση με τις γονικές `Tsk.Start` και `Tsk.Finish` ημερομηνίες, λαμβάνοντας υπόψη τα `Project.TaskLinks`. |
| [AsSoonAsPossible](#AsSoonAsPossible) | `Tsk.Start` και `Tsk.Finish` ημερομηνίες του `Task` προγραμματίζονται ASAP σε σχέση με τις γονικές `Tsk.Start` και `Tsk.Finish` ημερομηνίες, λαμβάνοντας υπόψη τα `Project.TaskLinks`. |
| [FinishNoEarlierThan](#FinishNoEarlierThan) | Ολοκλήρωση όχι νωρίτερα από |
| [FinishNoLaterThan](#FinishNoLaterThan) | Ολοκλήρωση όχι αργότερα από |
| [MustFinishOn](#MustFinishOn) | Πρέπει να ολοκληρωθεί στις |
| [MustStartOn](#MustStartOn) | Πρέπει να ξεκινήσει στις |
| [StartNoEarlierThan](#StartNoEarlierThan) | Έναρξη όχι νωρίτερα από |
| [StartNoLaterThan](#StartNoLaterThan) | Έναρξη όχι αργότερα από |
| [Undefined](#Undefined) | Η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
### AsLateAsPossible {#AsLateAsPossible}
```
public static final int AsLateAsPossible
```


`Tsk.Start` και `Tsk.Finish` ημερομηνίες του `Task` προγραμματίζονται ALAP σε σχέση με τις γονικές `Tsk.Start` και `Tsk.Finish` ημερομηνίες, λαμβάνοντας υπόψη τα `Project.TaskLinks`.

### AsSoonAsPossible {#AsSoonAsPossible}
```
public static final int AsSoonAsPossible
```


`Tsk.Start` και `Tsk.Finish` ημερομηνίες του `Task` προγραμματίζονται ASAP σε σχέση με τις γονικές `Tsk.Start` και `Tsk.Finish` ημερομηνίες, λαμβάνοντας υπόψη τα `Project.TaskLinks`.

### FinishNoEarlierThan {#FinishNoEarlierThan}
```
public static final int FinishNoEarlierThan
```


Ολοκλήρωση όχι νωρίτερα από

### FinishNoLaterThan {#FinishNoLaterThan}
```
public static final int FinishNoLaterThan
```


Ολοκλήρωση όχι αργότερα από

### MustFinishOn {#MustFinishOn}
```
public static final int MustFinishOn
```


Πρέπει να ολοκληρωθεί στις

### MustStartOn {#MustStartOn}
```
public static final int MustStartOn
```


Πρέπει να ξεκινήσει στις

### StartNoEarlierThan {#StartNoEarlierThan}
```
public static final int StartNoEarlierThan
```


Έναρξη όχι νωρίτερα από

### StartNoLaterThan {#StartNoLaterThan}
```
public static final int StartNoLaterThan
```


Έναρξη όχι αργότερα από

### Undefined {#Undefined}
```
public static final int Undefined
```


Η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου.


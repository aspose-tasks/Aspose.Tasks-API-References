---
title: "RiskItemStatistics"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει ένα στοιχείο που αποθηκεύει στατιστικά δεδομένα για την εργασία του αναλυθέντος έργου."
type: docs
weight: 265
url: /el/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Αντιπροσωπεύει ένα στοιχείο που αποθηκεύει στατιστικά δεδομένα για την εργασία του αναλυθέντος έργου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Επιστρέφει την αναμενόμενη τιμή του στοιχείου κινδύνου. |
| [getItemType()](#getItemType--) | Επιστρέφει μια παρουσία της απαρίθμησης [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | Επιστρέφει τη μέγιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo. |
| [getMinimum()](#getMinimum--) | Επιστρέφει τη ελάχιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo. |
| [getPercentile(int percent)](#getPercentile-int-) | Επιστρέφει μια τιμή κάτω από την οποία πέφτει ένα καθορισμένο ποσοστό των παραγόμενων δειγμάτων. |
| [getStandardDeviation()](#getStandardDeviation--) | Επιστρέφει την τυπική απόκλιση του στοιχείου κινδύνου. |
| [toString()](#toString--) | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός στοιχείου κινδύνου. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Επιστρέφει την αναμενόμενη τιμή του στοιχείου κινδύνου.

**Returns:**
java.util.Date - η αναμενόμενη τιμή του στοιχείου κινδύνου.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Επιστρέφει μια παρουσία της απαρίθμησης [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - ένα στιγμιότυπο της απαρίθμησης [RiskItemType](../../com.aspose/tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Επιστρέφει τη μέγιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo.

**Returns:**
java.util.Date - η μέγιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Επιστρέφει τη ελάχιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo.

**Returns:**
java.util.Date - η ελάχιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Επιστρέφει μια τιμή κάτω από την οποία πέφτει ένα καθορισμένο ποσοστό των παραγόμενων δειγμάτων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ποσοστό | int | το καθορισμένο ποσοστό μεταξύ 0 και 100. |

**Returns:**
java.util.Date - μια τιμή κάτω από την οποία πέφτει ένα καθορισμένο ποσοστό των παραγόμενων δειγμάτων.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Επιστρέφει την τυπική απόκλιση του στοιχείου κινδύνου.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός στοιχείου κινδύνου. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν καθορίζονται και ενδέχεται να αλλάξουν.

**Returns:**
java.lang.String - σύντομη συμβολοσειρά που αντιπροσωπεύει το αντικείμενο RiskItem.

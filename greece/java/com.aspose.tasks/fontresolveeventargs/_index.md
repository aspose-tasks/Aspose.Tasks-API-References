---
title: "FontResolveEventArgs"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Παρέχει επιχειρήματα για την κλήση που ενεργοποιείται όταν η γραμματοσειρά επιλύεται."
type: docs
weight: 99
url: /el/java/com.aspose.tasks/fontresolveeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public final class FontResolveEventArgs extends System.EventArgs
```

Παρέχει επιχειρήματα για την κλήση που ενεργοποιείται όταν η γραμματοσειρά επιλύεται.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getRequestedFontName()](#getRequestedFontName--) | Αποκτά το όνομα της ζητούμενης γραμματοσειράς. |
| [getResolvedFontName()](#getResolvedFontName--) | Αποκτά το όνομα της επιλυμένης γραμματοσειράς. |
| [setResolvedFontName(String value)](#setResolvedFontName-java.lang.String-) | Ορίζει το όνομα της επιλυμένης γραμματοσειράς. |
### getRequestedFontName() {#getRequestedFontName--}
```
public final String getRequestedFontName()
```


Αποκτά το όνομα της ζητούμενης γραμματοσειράς.

**Returns:**
java.lang.String - το όνομα της ζητούμενης γραμματοσειράς.
### getResolvedFontName() {#getResolvedFontName--}
```
public final String getResolvedFontName()
```


Αποκτά το όνομα της επιλυμένης γραμματοσειράς. Μπορεί να οριστεί για να ελέγχει τις γραμματοσειρές που χρησιμοποιούνται για την απόδοση μιας προβολής.

**Returns:**
java.lang.String - Όνομα της ζητούμενης γραμματοσειράς εάν βρεθεί ή όνομα της εναλλακτικής γραμματοσειράς ή null εάν η γραμματοσειρά δεν μπορεί να βρεθεί.
### setResolvedFontName(String value) {#setResolvedFontName-java.lang.String-}
```
public final void setResolvedFontName(String value)
```


Ορίζει το όνομα της επιλυμένης γραμματοσειράς. Μπορεί να οριστεί για να ελέγχει τις γραμματοσειρές που χρησιμοποιούνται για την απόδοση μιας προβολής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα της επιλυμένης γραμματοσειράς. |


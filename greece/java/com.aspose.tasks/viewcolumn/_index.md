---
title: "ViewColumn"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια στήλη σε μια προβολή έργου."
type: docs
weight: 344
url: /el/java/com.aspose.tasks/viewcolumn/
---

**Inheritance:**
java.lang.Object
```
public abstract class ViewColumn
```

Αναπαριστά μια στήλη σε μια προβολή έργου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getField()](#getField--) | Λαμβάνει το πεδίο της στήλης. |
| [getName()](#getName--) | Λαμβάνει το όνομα της στήλης. |
| [getStringAlignment()](#getStringAlignment--) | Λαμβάνει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getTextStyleModificationCallback()](#getTextStyleModificationCallback--) | Λαμβάνει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
| [getWidth()](#getWidth--) | Λαμβάνει το πλάτος της στήλης. |
| [setField(int value)](#setField-int-) | Ορίζει το πεδίο της στήλης. |
| [setStringAlignment(int value)](#setStringAlignment-int-) | Ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) απαρίθμησης). |
| [setTextStyleModificationCallback(ITextStyleModificationCallback value)](#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-) | Ορίζει το callback που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
### getField() {#getField--}
```
public abstract int getField()
```


Λαμβάνει το πεδίο της στήλης. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Returns:**
int - πεδίο στήλης.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα της στήλης.

**Returns:**
java.lang.String - το όνομα της στήλης.
### getStringAlignment() {#getStringAlignment--}
```
public final int getStringAlignment()
```


Λαμβάνει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) απαρίθμησης).
### getTextStyleModificationCallback() {#getTextStyleModificationCallback--}
```
public final ITextStyleModificationCallback getTextStyleModificationCallback()
```


Λαμβάνει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης.

**Returns:**
[ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) - the callback which can be used to customize the appearance of the column's cells.
### getWidth() {#getWidth--}
```
public final int getWidth()
```


Λαμβάνει το πλάτος της στήλης.

**Returns:**
int - το πλάτος της στήλης.
### setField(int value) {#setField-int-}
```
public abstract void setField(int value)
```


Ορίζει το πεδίο της στήλης. `Field`([getField()](../../com.aspose.tasks/viewcolumn\#getField--)/[setField(int)](../../com.aspose.tasks/viewcolumn\#setField-int-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | πεδίο στήλης. |

### setStringAlignment(int value) {#setStringAlignment-int-}
```
public final void setStringAlignment(int value)
```


Ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της [HorizontalStringAlignment](../../com.aspose/tasks/horizontalstringalignment) απαρίθμησης).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | int | ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της [HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment) απαρίθμησης). |

### setTextStyleModificationCallback(ITextStyleModificationCallback value) {#setTextStyleModificationCallback-com.aspose.tasks.ITextStyleModificationCallback-}
```
public final void setTextStyleModificationCallback(ITextStyleModificationCallback value)
```


Ορίζει το callback που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ITextStyleModificationCallback](../../com.aspose.tasks/itextstylemodificationcallback) | το callback που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |


---
title: "ResourceSavingArgs"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την αποθήκευση εξωτερικών αρχείων πόρων που πραγματοποιείται κατά τη μετατροπή σε μορφή HTML."
type: docs
weight: 254
url: /el/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Αυτή η κλάση αντιπροσωπεύει ένα σύνολο δεδομένων που σχετίζονται με την αποθήκευση εξωτερικού αρχείου πόρων που συμβαίνει κατά τη μετατροπή σε μορφή HTML.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | Κλείστε τη ροή εάν KeepStreamOpen είναι ψευδές, αλλιώς αδειάστε την. |
| [getFileName()](#getFileName--) | Λαμβάνει το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων. |
| [getStream()](#getStream--) | Λαμβάνει το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου. |
| [getUri()](#getUri--) | Λαμβάνει το URI του πόρου. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Ορίζει το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Ορίζει το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου. |
| [setUri(String value)](#setUri-java.lang.String-) | Ορίζει το URI του πόρου. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


Κλείστε τη ροή εάν KeepStreamOpen είναι ψευδές, αλλιώς αδειάστε την.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Λαμβάνει το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. Μπορεί να χρησιμοποιηθεί σε προσαρμοσμένο κώδικα για να αποφασίσει πώς να επεξεργαστεί ή πού να αποθηκεύσει το αρχείο.

**Returns:**
java.lang.String - το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Λαμβάνει το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου.

**Returns:**
java.io.OutputStream - το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου.
### getUri() {#getUri--}
```
public final String getUri()
```


Λαμβάνει το URI του πόρου.

**Returns:**
java.lang.String - το URI του πόρου.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Ορίζει το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. Μπορεί να χρησιμοποιηθεί σε προσαρμοσμένο κώδικα για να αποφασίσει πώς να επεξεργαστεί ή πού να αποθηκεύσει το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το υποτιθέμενο όνομα αρχείου που περνά από τον μετατροπέα στον κώδικα της προσαρμοσμένης μεθόδου. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν η ροή θα παραμείνει ανοιχτή μετά το τέλος της αποθήκευσης πόρων. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Ορίζει το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.io.OutputStream | το δυαδικό περιεχόμενο του αποθηκευμένου αρχείου. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Ορίζει το URI του πόρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το URI του πόρου. |


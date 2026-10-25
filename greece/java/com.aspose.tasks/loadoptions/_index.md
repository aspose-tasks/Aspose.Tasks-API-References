---
title: "LoadOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων παραμέτρων φόρτωσης κατά τη φόρτωση ενός έργου από αρχείο ή ροή."
type: docs
weight: 148
url: /el/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Επιτρέπει τον καθορισμό πρόσθετων παραμέτρων φόρτωσης κατά τη φόρτωση ενός έργου από αρχείο ή ροή.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Λαμβάνει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου. |
| [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. |
| [getErrorHandler()](#getErrorHandler--) | Λαμβάνει μια μέθοδο callback για τη διαχείριση σφαλμάτων ανάλυσης xml. |
| [getPassword()](#getPassword--) | Λαμβάνει έναν κωδικό προστασίας. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Λαμβάνει μια καθορισμένη παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml). |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | Ορίζει μια μέθοδο callback για τη διαχείριση σφαλμάτων ανάλυσης xml. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ορίζει έναν κωδικό προστασίας. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Ορίζει μια καθορισμένη παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml). |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LoadOptions](../../com.aspose.tasks/loadoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Λαμβάνει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. Η προεπιλεγμένη κωδικοποίηση είναι UTF8.

**Returns:**
java.nio.charset.Charset - η κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


Λαμβάνει μια μέθοδο callback για τη διαχείριση σφαλμάτων ανάλυσης xml.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Λαμβάνει έναν κωδικό προστασίας.

**Returns:**
java.lang.String - ένας κωδικός προστασίας.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Λαμβάνει μια καθορισμένη παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml).

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ορίζει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. Η προεπιλεγμένη κωδικοποίηση είναι UTF8.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.nio.charset.Charset | η κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


Ορίζει μια μέθοδο callback για τη διαχείριση σφαλμάτων ανάλυσης xml.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | μια μέθοδος callback για τη διαχείριση σφαλμάτων ανάλυσης xml. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ορίζει έναν κωδικό προστασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ένας κωδικός προστασίας. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Ορίζει μια καθορισμένη παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | μια καθορισμένη παρουσία της κλάσης [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της συμπεριφοράς φόρτωσης μορφών Primavera (Primavera P6 XER ή Primavera P6 Xml). |


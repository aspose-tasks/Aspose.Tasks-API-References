---
title: "PrinterSettings"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Καθορίζει πληροφορίες σχετικά με το πώς εκτυπώνεται ένα έγγραφο, συμπεριλαμβανομένου του εκτυπωτή που το εκτυπώνει."
type: docs
weight: 215
url: /el/java/com.aspose.tasks/printersettings/
---

**Inheritance:**
java.lang.Object
```
public class PrinterSettings
```

Καθορίζει πληροφορίες σχετικά με το πώς εκτυπώνεται ένα έγγραφο, συμπεριλαμβανομένου του εκτυπωτή που το εκτυπώνει.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PrinterSettings()](#PrinterSettings--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCollate()](#getCollate--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο. |
| [getCopies()](#getCopies--) | Λαμβάνει τον αριθμό των αντιτύπων του εγγράφου που θα εκτυπωθούν. |
| [getFromPage()](#getFromPage--) | Λαμβάνει τον αριθμό σελίδας της πρώτης σελίδας προς εκτύπωση. |
| [getPrintFileName()](#getPrintFileName--) | Λαμβάνει το όνομα του αρχείου, όταν εκτυπώνεται σε αρχείο. |
| [getPrinterName()](#getPrinterName--) | Λαμβάνει το όνομα του εκτυπωτή που θα χρησιμοποιηθεί. |
| [getSupportsColor()](#getSupportsColor--) | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο εκτυπωτής υποστηρίζει έγχρωμη εκτύπωση. |
| [getToPage()](#getToPage--) | Λαμβάνει τον αριθμό της τελευταίας σελίδας προς εκτύπωση. |
| [isDefaultPrinter()](#isDefaultPrinter--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PrinterName ορίζει τον προεπιλεγμένο εκτυπωτή, εκτός εάν ο χρήστης ορίζει ρητά το PrinterName. |
| [setCollate(boolean value)](#setCollate-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο. |
| [setCopies(short value)](#setCopies-short-) | Ορίζει τον αριθμό των αντιτύπων του εγγράφου που θα εκτυπωθούν. |
| [setFromPage(int value)](#setFromPage-int-) | Ορίζει τον αριθμό σελίδας της πρώτης σελίδας προς εκτύπωση. |
| [setPrintFileName(String value)](#setPrintFileName-java.lang.String-) | Ορίζει το όνομα του αρχείου, όταν εκτυπώνεται σε αρχείο. |
| [setPrinterName(String value)](#setPrinterName-java.lang.String-) | Ορίζει το όνομα του εκτυπωτή που θα χρησιμοποιηθεί. |
| [setToPage(int value)](#setToPage-int-) | Ορίζει τον αριθμό της τελευταίας σελίδας προς εκτύπωση. |
| [toString()](#toString--) | Παρέχει πληροφορίες σχετικά με το PrinterSettings σε μορφή συμβολοσειράς. |
### PrinterSettings() {#PrinterSettings--}
```
public PrinterSettings()
```


### getCollate() {#getCollate--}
```
public boolean getCollate()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο.
### getCopies() {#getCopies--}
```
public short getCopies()
```


Λαμβάνει τον αριθμό των αντιτύπων του εγγράφου που θα εκτυπωθούν.

**Returns:**
short - ο αριθμός των αντιτύπων του εγγράφου που θα εκτυπωθούν.
### getFromPage() {#getFromPage--}
```
public int getFromPage()
```


Λαμβάνει τον αριθμό σελίδας της πρώτης σελίδας προς εκτύπωση.

**Returns:**
int - ο αριθμός σελίδας της πρώτης σελίδας προς εκτύπωση.
### getPrintFileName() {#getPrintFileName--}
```
public String getPrintFileName()
```


Λαμβάνει το όνομα του αρχείου, όταν εκτυπώνεται σε αρχείο.

**Returns:**
java.lang.String - το όνομα αρχείου, όταν εκτυπώνεται σε αρχείο.
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```


Λαμβάνει το όνομα του εκτυπωτή που θα χρησιμοποιηθεί.

**Returns:**
java.lang.String - το όνομα του εκτυπωτή που θα χρησιμοποιηθεί.
### getSupportsColor() {#getSupportsColor--}
```
public boolean getSupportsColor()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν αυτός ο εκτυπωτής υποστηρίζει έγχρωμη εκτύπωση.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν αυτός ο εκτυπωτής υποστηρίζει εκτύπωση χρώματος.
### getToPage() {#getToPage--}
```
public int getToPage()
```


Λαμβάνει τον αριθμό της τελευταίας σελίδας προς εκτύπωση.

**Returns:**
int - ο αριθμός της τελευταίας σελίδας για εκτύπωση.
### isDefaultPrinter() {#isDefaultPrinter--}
```
public boolean isDefaultPrinter()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PrinterName ορίζει τον προεπιλεγμένο εκτυπωτή, εκτός εάν ο χρήστης ορίζει ρητά το PrinterName.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η ιδιότητα PrinterName ορίζει τον προεπιλεγμένο εκτυπωτή.
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν το εκτυπωμένο έγγραφο είναι ταξινομημένο. |

### setCopies(short value) {#setCopies-short-}
```
public void setCopies(short value)
```


Ορίζει τον αριθμό των αντιτύπων του εγγράφου που θα εκτυπωθούν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | short | ο αριθμός των αντιτύπων του εγγράφου για εκτύπωση. |

### setFromPage(int value) {#setFromPage-int-}
```
public void setFromPage(int value)
```


Ορίζει τον αριθμό σελίδας της πρώτης σελίδας προς εκτύπωση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο αριθμός σελίδας της πρώτης σελίδας για εκτύπωση. |

### setPrintFileName(String value) {#setPrintFileName-java.lang.String-}
```
public void setPrintFileName(String value)
```


Ορίζει το όνομα του αρχείου, όταν εκτυπώνεται σε αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα αρχείου, όταν εκτυπώνεται σε αρχείο. |

### setPrinterName(String value) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String value)
```


Ορίζει το όνομα του εκτυπωτή που θα χρησιμοποιηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το όνομα του εκτυπωτή που θα χρησιμοποιηθεί. |

### setToPage(int value) {#setToPage-int-}
```
public void setToPage(int value)
```


Ορίζει τον αριθμό της τελευταίας σελίδας προς εκτύπωση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο αριθμός της τελευταίας σελίδας για εκτύπωση. |

### toString() {#toString--}
```
public String toString()
```


Παρέχει πληροφορίες σχετικά με το PrinterSettings σε μορφή συμβολοσειράς.

**Returns:**
java.lang.String - πληροφορίες σχετικά με τις ρυθμίσεις του PrinterSettings σε μορφή συμβολοσειράς.

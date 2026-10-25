---
title: "Τιμή"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια τιμή σε μια λίστα τιμών."
type: docs
weight: 333
url: /el/java/com.aspose.tasks/value/
---

**Inheritance:**
java.lang.Object
```
public class Value
```

Αναπαριστά μια τιμή σε μια λίστα τιμών.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Value()](#Value--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Value](../../com.aspose/tasks/value). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDateValue()](#getDateValue--) | Λαμβάνει την πραγματική τιμή αν μπορεί να αναπαρασταθεί ως DateTime. |
| [getDescription()](#getDescription--) | Λαμβάνει την περιγραφή μιας τιμής. |
| [getDuration()](#getDuration--) | Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση της Διάρκειας. |
| [getId()](#getId--) | Λαμβάνει το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο. |
| [getNumericValue()](#getNumericValue--) | Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους. |
| [getPhonetic()](#getPhonetic--) | Λαμβάνει τις φωνητικές πληροφορίες για το όνομα προσαρμοσμένου πεδίου. |
| [getStringValue()](#getStringValue--) | Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση συμβολοσειράς κειμένου. |
| [getVal()](#getVal--) | Λαμβάνει την πραγματική τιμή σε εσωτερική αναπαράσταση. |
| [getValueGuid()](#getValueGuid--) | Λαμβάνει ένα GUID που αναγνωρίζει αυτήν την τιμή μεταξύ των άλλων σε ολόκληρο το έργο. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Ορίζει την πραγματική τιμή αν μπορεί να αναπαρασταθεί ως DateTime. |
| [setDescription(String value)](#setDescription-java.lang.String-) | Ορίζει την περιγραφή μιας τιμής. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση της Διάρκειας. |
| [setId(int value)](#setId-int-) | Ορίζει το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους. |
| [setPhonetic(String value)](#setPhonetic-java.lang.String-) | Ορίζει τις φωνητικές πληροφορίες για το όνομα προσαρμοσμένου πεδίου. |
| [setStringValue(String value)](#setStringValue-java.lang.String-) | Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση συμβολοσειράς κειμένου. |
| [setVal(String value)](#setVal-java.lang.String-) | Ορίζει την πραγματική τιμή σε εσωτερική αναπαράσταση. |
### Value() {#Value--}
```
public Value()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Value](../../com.aspose/tasks/value).

### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Λαμβάνει την πραγματική τιμή αν μπορεί να αναπαρασταθεί ως DateTime. Η προεπιλεγμένη τιμή είναι DateTime\#MinValue.MinValue.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή DateTime.

**Returns:**
java.util.Date - η πραγματική τιμή εάν μπορεί να αναπαρασταθεί ως DateTime.
### getDescription() {#getDescription--}
```
public final String getDescription()
```


Λαμβάνει την περιγραφή μιας τιμής.

**Returns:**
java.lang.String - η περιγραφή μιας τιμής.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση της Διάρκειας.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Duration.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the actual value which is used to represent Duration.
### getId() {#getId--}
```
public final int getId()
```


Λαμβάνει το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο.

Είναι σημαντικό να μην υπάρχουν τα ίδια αναγνωριστικά για διαφορετικές περιπτώσεις του [Value](../../com.aspose.tasks/value).

Η ελάχιστη τιμή του `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) είναι `1`.

**Returns:**
int - το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Number ή Cost.

**Returns:**
java.math.BigDecimal - η πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους.
### getPhonetic() {#getPhonetic--}
```
public final String getPhonetic()
```


Λαμβάνει τις φωνητικές πληροφορίες για το όνομα προσαρμοσμένου πεδίου.

**Returns:**
java.lang.String - η φωνητική πληροφορία για το όνομα προσαρμοσμένου πεδίου.
### getStringValue() {#getStringValue--}
```
public final String getStringValue()
```


Λαμβάνει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση συμβολοσειράς κειμένου.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Text.

**Returns:**
java.lang.String - η πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση της συμβολοσειράς Text.
### getVal() {#getVal--}
```
public final String getVal()
```


Αποκτά την πραγματική τιμή στην εσωτερική αναπαράσταση. Προτιμήστε τη χρήση ιδιοτήτων έντονης τυποποίησης που αναφέρονται παρακάτω.

--------------------

Αν θέλετε να ορίσετε την τιμή Text, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) property.

Αν θέλετε να ορίσετε την τιμή Number ή Cost, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) property.

Αν θέλετε να ορίσετε τιμές Date/Start/Finish, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `DateValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)) property.

Αν θέλετε να ορίσετε την τιμή Duration, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) property.

Εάν ο τύπος σας δεν αναφέρεται, χρησιμοποιήστε την ιδιότητα `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) property.

**Returns:**
java.lang.String - η πραγματική τιμή στην εσωτερική αναπαράσταση.
### getValueGuid() {#getValueGuid--}
```
public final UUID getValueGuid()
```


Λαμβάνει ένα GUID που αναγνωρίζει αυτήν την τιμή μεταξύ των άλλων σε ολόκληρο το έργο.

**Returns:**
java.util.UUID - ένα GUID που αναγνωρίζει αυτήν την τιμή μεταξύ των άλλων σε ολόκληρο το έργο.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Ορίζει την πραγματική τιμή εάν μπορεί να αναπαρασταθεί ως DateTime. Η προεπιλεγμένη τιμή είναι DateTime\#MinValue.MinValue.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή DateTime.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η πραγματική τιμή εάν μπορεί να αναπαρασταθεί ως DateTime. |

### setDescription(String value) {#setDescription-java.lang.String-}
```
public final void setDescription(String value)
```


Ορίζει την περιγραφή μιας τιμής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η περιγραφή μιας τιμής. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση της Διάρκειας.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Duration.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | η πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση του Duration. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Ορίζει το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο.

Είναι σημαντικό να μην υπάρχουν τα ίδια αναγνωριστικά για διαφορετικές περιπτώσεις του [Value](../../com.aspose.tasks/value).

Η ελάχιστη τιμή του `Id`([getId()](../../com.aspose/tasks/value\#getId--)/[setId(int)](../../com.aspose/tasks/value\#setId-int-)) είναι `1`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοναδικό αναγνωριστικό μιας τιμής σε όλο το έργο. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Number ή Cost.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | η πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση αριθμού ή τιμής κόστους. |

### setPhonetic(String value) {#setPhonetic-java.lang.String-}
```
public final void setPhonetic(String value)
```


Ορίζει τις φωνητικές πληροφορίες για το όνομα προσαρμοσμένου πεδίου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η φωνητική πληροφορία για το όνομα προσαρμοσμένου πεδίου. |

### setStringValue(String value) {#setStringValue-java.lang.String-}
```
public final void setStringValue(String value)
```


Ορίζει την πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση συμβολοσειράς κειμένου.

--------------------

Προτιμήστε αυτήν την ιδιότητα αντί της `Val`([getVal()](../../com.aspose/tasks/value\#getVal--)/[setVal(String)](../../com.aspose/tasks/value\#setVal-String-)), όταν χρειάζεται να ορίσετε την τιμή Text.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η πραγματική τιμή που χρησιμοποιείται για την αναπαράσταση συμβολοσειράς κειμένου. |

### setVal(String value) {#setVal-java.lang.String-}
```
public final void setVal(String value)
```


Ορίζει την πραγματική τιμή στην εσωτερική αναπαράσταση. Προτιμήστε τη χρήση ισχυρά τυποποιημένων ιδιοτήτων που παρατίθενται παρακάτω.

--------------------

Αν θέλετε να ορίσετε την τιμή Text, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `StringValue`([getStringValue()](../../com.aspose.tasks/value\#getStringValue--)/[setStringValue(String)](../../com.aspose.tasks/value\#setStringValue-String-)) property.

Αν θέλετε να ορίσετε την τιμή Number ή Cost, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `NumericValue`([getNumericValue()](../../com.aspose.tasks/value\#getNumericValue--)/[setNumericValue(java.math.BigDecimal)](../../com.aspose.tasks/value\#setNumericValue-java.math.BigDecimal-)) property.

Εάν θέλετε να ορίσετε τιμές Ημερομηνίας/Έναρξης/Λήξης, προτιμήστε τη χρήση ισχυρά τυποποιημένης ιδιότητας `DateTimeValue`([getDateValue()](../../com.aspose.tasks/value\#getDateValue--)/[setDateValue(java.util.Date)](../../com.aspose.tasks/value\#setDateValue-java.util.Date-)).

Αν θέλετε να ορίσετε την τιμή Duration, προτιμήστε τη χρήση της έντονα τυποποιημένης ιδιότητας `Duration`([getDuration()](../../com.aspose.tasks/value\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/value\#setDuration-Duration-)) property.

Εάν ο τύπος σας δεν αναφέρεται, χρησιμοποιήστε την ιδιότητα `Val`([getVal()](../../com.aspose.tasks/value\#getVal--)/[setVal(String)](../../com.aspose.tasks/value\#setVal-String-)) property.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η πραγματική τιμή στην εσωτερική αναπαράσταση. |


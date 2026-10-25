---
title: "TimephasedData"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά δεδομένα χρονικής φάσης."
type: docs
weight: 320
url: /el/java/com.aspose.tasks/timephaseddata/
---

**Inheritance:**
java.lang.Object
```
public class TimephasedData
```

Αναπαριστά δεδομένα χρονικής φάσης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TimephasedData()](#TimephasedData--) | Αρχικοποιεί μια νέα παρουσία της [TimephasedData](../../com.aspose.tasks/timephaseddata) κλάσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει κόστους. |
| [createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει κόστους. |
| [createUnitTimephased(int uid, Date start, Date finish, double units, byte type)](#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει μονάδας μιας ανάθεσης υλικού πόρου. |
| [createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)](#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-) | Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει εργασίας. |
| [getFinish()](#getFinish--) | Λαμβάνει την ημερομηνία λήξης μιας περιόδου χρονομερισμένων δεδομένων. |
| [getStart()](#getStart--) | Λαμβάνει την ημερομηνία έναρξης μιας περιόδου χρονομερισμένων δεδομένων. |
| [getTimephasedDataType()](#getTimephasedDataType--) | Λαμβάνει τον τύπο ενός χρονομερισμένου δεδομένου. |
| [getUid()](#getUid--) | Λαμβάνει το μοναδικό αναγνωριστικό ενός χρονομερισμένου δεδομένου |
| [getUnit()](#getUnit--) | Λαμβάνει τη μονάδα χρόνου μιας περιόδου χρονομερισμένων δεδομένων. |
| [getValue()](#getValue--) | Λαμβάνει την τιμή ανά μονάδα χρόνου για μια περίοδο χρονομερισμένων δεδομένων. |
| [getValueToCost()](#getValueToCost--) | Λαμβάνει το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου. |
| [getValueToDuration()](#getValueToDuration--) | Λαμβάνει το αντικείμενο double που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου. |
| [getValueToUnits()](#getValueToUnits--) | Λαμβάνει το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου για δεδομένα χρονομερισμένα βάσει μονάδας. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Ορίζει την ημερομηνία λήξης μιας περιόδου χρονομερισμένων δεδομένων. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ορίζει την ημερομηνία έναρξης μιας περιόδου χρονομερισμένων δεδομένων. |
| [setTimephasedDataType(byte value)](#setTimephasedDataType-byte-) | Ορίζει τον τύπο ενός χρονομερισμένου δεδομένου. |
| [setUid(int value)](#setUid-int-) | Ορίζει το μοναδικό αναγνωριστικό ενός χρονομερισμένου δεδομένου |
| [setUnit(byte value)](#setUnit-byte-) | Ορίζει τη μονάδα χρόνου μιας περιόδου χρονομερισμένων δεδομένων. |
| [setValue(String value)](#setValue-java.lang.String-) | Ορίζει την τιμή ανά μονάδα χρόνου για μια περίοδο χρονομερισμένων δεδομένων. |
| [setValueToCost(double value)](#setValueToCost-double-) | Το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου. |
### TimephasedData() {#TimephasedData--}
```
public TimephasedData()
```


Αρχικοποιεί μια νέα παρουσία της [TimephasedData](../../com.aspose.tasks/timephaseddata) κλάσης.

### createCostTimephased(int uid, Date start, Date finish, double value, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte type)
```


Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει κόστους.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | Αναγνωριστικό UID της εργασίας. |
| έναρξη | java.util.Date | ημερομηνία-ώρα έναρξης. |
| λήξη | java.util.Date | Ημερομηνία-ώρα λήξης. |
| τιμή | double | Τιμή κόστους. |
| type | byte | Τύπος χρονομερισμένων δεδομένων. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createCostTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createCostTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει κόστους.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | Αναγνωριστικό UID της εργασίας. |
| έναρξη | java.util.Date | ημερομηνία-ώρα έναρξης. |
| λήξη | java.util.Date | Ημερομηνία-ώρα λήξης. |
| τιμή | double | Τιμή κόστους. |
| μονάδα χρόνου | byte | Τύπος μονάδας χρόνου. |
| type | byte | Τύπος χρονομερισμένων δεδομένων. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createUnitTimephased(int uid, Date start, Date finish, double units, byte type) {#createUnitTimephased-int-java.util.Date-java.util.Date-double-byte-}
```
public static TimephasedData createUnitTimephased(int uid, Date start, Date finish, double units, byte type)
```


Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει μονάδας μιας ανάθεσης υλικού πόρου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | Αναγνωριστικό UID της εργασίας. |
| έναρξη | java.util.Date | Η ημερομηνία-ώρα έναρξης. |
| λήξη | java.util.Date | Ημερομηνία-ώρα λήξης. |
| μονάδες | double | Αριθμός μονάδων. |
| type | byte | Τύπος χρονομερισμένων δεδομένων. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for cost-based time phased data.
### createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type) {#createWorkTimephased-int-java.util.Date-java.util.Date-double-byte-byte-}
```
public static TimephasedData createWorkTimephased(int uid, Date start, Date finish, double value, byte timeUnit, byte type)
```


Δημιουργεί και αρχικοποιεί μια νέα παρουσία της κλάσης [TimephasedData](../../com.aspose.tasks/timephaseddata) για δεδομένα χρονομερισμένα βάσει εργασίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| uid | int | Αναγνωριστικό UID της εργασίας. |
| έναρξη | java.util.Date | ημερομηνία-ώρα έναρξης. |
| λήξη | java.util.Date | Ημερομηνία-ώρα λήξης. |
| τιμή | double | Τιμή χρονικού διαστήματος. |
| μονάδα χρόνου | byte | Τύπος μονάδας χρόνου. |
| type | byte | Τύπος χρονομερισμένων δεδομένων. |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - A instance of the [TimephasedData](../../com.aspose.tasks/timephaseddata) class for work-based time phased data.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Λαμβάνει την ημερομηνία λήξης μιας περιόδου χρονομερισμένων δεδομένων.

**Returns:**
java.util.Date - η ημερομηνία λήξης μιας περιόδου δεδομένων με χρονική φάση.
### getStart() {#getStart--}
```
public final Date getStart()
```


Λαμβάνει την ημερομηνία έναρξης μιας περιόδου χρονομερισμένων δεδομένων.

**Returns:**
java.util.Date - η ημερομηνία έναρξης μιας περιόδου δεδομένων με χρονική φάση.
### getTimephasedDataType() {#getTimephasedDataType--}
```
public final byte getTimephasedDataType()
```


Λαμβάνει τον τύπο ενός χρονομερισμένου δεδομένου.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) η ιδιότητα θα καθαριστεί, εάν δεν είναι κατάλληλη για τον τύπο που καθορίζεται εδώ.

**Returns:**
byte - ο τύπος ενός δεδομένου με χρονική φάση.
### getUid() {#getUid--}
```
public final int getUid()
```


Λαμβάνει το μοναδικό αναγνωριστικό ενός χρονομερισμένου δεδομένου

**Returns:**
int - το μοναδικό αναγνωριστικό ενός δεδομένου με χρονική φάση
### getUnit() {#getUnit--}
```
public final byte getUnit()
```


Λαμβάνει τη μονάδα χρόνου μιας περιόδου χρονομερισμένων δεδομένων.

**Returns:**
byte - η μονάδα χρόνου μιας περιόδου δεδομένων με χρονική φάση.
### getValue() {#getValue--}
```
public final String getValue()
```


Λαμβάνει την τιμή ανά μονάδα χρόνου για μια περίοδο χρονομερισμένων δεδομένων.

**Returns:**
java.lang.String - η τιμή ανά μονάδα χρόνου για μια περίοδο δεδομένων με χρονική φάση.
### getValueToCost() {#getValueToCost--}
```
public final double getValueToCost()
```


Λαμβάνει το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου.

**Returns:**
double - μια αναπαράσταση κινητής υποδιαστολής του αντικειμένου.
### getValueToDuration() {#getValueToDuration--}
```
public final double getValueToDuration()
```


Λαμβάνει το αντικείμενο double που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου.

**Returns:**
double - μια αναπαράσταση χρονικού διαστήματος του αντικειμένου.
### getValueToUnits() {#getValueToUnits--}
```
public final double getValueToUnits()
```


Λαμβάνει το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου για δεδομένα χρονομερισμένα βάσει μονάδας.

**Returns:**
double - μια αναπαράσταση κινητής υποδιαστολής αυτού του αντικειμένου.
### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Ορίζει την ημερομηνία λήξης μιας περιόδου χρονομερισμένων δεδομένων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία λήξης μιας περιόδου δεδομένων με χρονική φάση. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ορίζει την ημερομηνία έναρξης μιας περιόδου χρονομερισμένων δεδομένων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | η ημερομηνία έναρξης μιας περιόδου δεδομένων με χρονική φάση. |

### setTimephasedDataType(byte value) {#setTimephasedDataType-byte-}
```
public final void setTimephasedDataType(byte value)
```


Ορίζει τον τύπο ενός χρονομερισμένου δεδομένου.

--------------------

`Value`([getValue()](../../com.aspose.tasks/timephaseddata\#getValue--)/[setValue(String)](../../com.aspose.tasks/timephaseddata\#setValue-String-)) η ιδιότητα θα καθαριστεί, εάν δεν είναι κατάλληλη για τον τύπο που καθορίζεται εδώ.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | byte | ο τύπος ενός δεδομένου με χρονική φάση. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ορίζει το μοναδικό αναγνωριστικό ενός χρονομερισμένου δεδομένου

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το μοναδικό αναγνωριστικό ενός δεδομένου με χρονική φάση |

### setUnit(byte value) {#setUnit-byte-}
```
public final void setUnit(byte value)
```


Ορίζει τη μονάδα χρόνου μιας περιόδου χρονομερισμένων δεδομένων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | byte | η μονάδα χρόνου μιας περιόδου δεδομένων με χρονική φάση. |

### setValue(String value) {#setValue-java.lang.String-}
```
public final void setValue(String value)
```


Ορίζει την τιμή ανά μονάδα χρόνου για μια περίοδο χρονομερισμένων δεδομένων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η τιμή ανά μονάδα χρόνου για μια περίοδο δεδομένων με χρονική φάση. |

### setValueToCost(double value) {#setValueToCost-double-}
```
public final void setValueToCost(double value)
```


Το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | Το αντικείμενο `double` που αντιπροσωπεύει την τιμή συμβολοσειράς αυτού του αντικειμένου. |


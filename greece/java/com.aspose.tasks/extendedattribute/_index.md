---
title: "ExtendedAttribute"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά επεκταμένα χαρακτηριστικά."
type: docs
weight: 81
url: /el/java/com.aspose.tasks/extendedattribute/
---

**Inheritance:**
java.lang.Object
```
public class ExtendedAttribute
```

Αναπαριστά επεκταμένα χαρακτηριστικά.

--------------------

Προς το παρόν υποστηρίζονται όλοι οι τύποι εκτεταμένων χαρακτηριστικών που διαβάζονται από MSP Xml 2003/2007 και mpp 2003. Για MSP mpp 2007 η ανάγνωση όλων των εκτεταμένων χαρακτηριστικών υποστηρίζεται εκτός από διάρκειες και σημαίες.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAttributeDefinition()](#getAttributeDefinition--) | Λαμβάνει τον ορισμό του χαρακτηριστικού. |
| [getDateValue()](#getDateValue--) | Λαμβάνει μια τιμή για χαρακτηριστικά με τύπους ημερομηνίας (Date, Start, Finish). |
| [getDurationValue()](#getDurationValue--) | Λαμβάνει την τιμή για ιδιότητες με τύπο 'Duration'. |
| [getFieldId()](#getFieldId--) | Λαμβάνει το αναγνωριστικό ενός πεδίου. |
| [getFlagValue()](#getFlagValue--) | Λαμβάνει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα με τύπο 'Flag'. |
| [getNumericValue()](#getNumericValue--) | Λαμβάνει μια τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number). |
| [getTextValue()](#getTextValue--) | Λαμβάνει μια τιμή για ιδιότητες με τύπο 'Text'. |
| [getValueGuid()](#getValueGuid--) | Λαμβάνει το guid μιας τιμής αναζήτησης. |
| [getValueReadOnly()](#getValueReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει εάν μια τιμή αυτού του αντικειμένου [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) είναι μόνο για ανάγνωση. |
| [isErrorValue()](#isErrorValue--) | Λαμβάνει εάν ο υπολογισμός της τιμής της εκτεταμένης ιδιότητας κατέληξε σε σφάλμα. |
| [setDateValue(Date value)](#setDateValue-java.util.Date-) | Ορίζει μια τιμή για ιδιότητες με τύπους ημερομηνίας (Date, Start, Finish). |
| [setDurationValue(Duration value)](#setDurationValue-com.aspose.tasks.Duration-) | Ορίζει τιμή για ιδιότητες με τύπο 'Duration'. |
| [setFlagValue(boolean value)](#setFlagValue-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα με τύπο 'Flag'. |
| [setNumericValue(BigDecimal value)](#setNumericValue-java.math.BigDecimal-) | Ορίζει μια τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number). |
| [setTextValue(String value)](#setTextValue-java.lang.String-) | Ορίζει μια τιμή για ιδιότητες με τύπο 'Text'. |
| [toString()](#toString--) | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς μιας εκτεταμένης ιδιότητας. |
### getAttributeDefinition() {#getAttributeDefinition--}
```
public final ExtendedAttributeDefinition getAttributeDefinition()
```


Λαμβάνει τον ορισμό του χαρακτηριστικού.

**Returns:**
[ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) - the attribute definition.
### getDateValue() {#getDateValue--}
```
public final Date getDateValue()
```


Λαμβάνει μια τιμή για χαρακτηριστικά με τύπους ημερομηνίας (Date, Start, Finish).

**Returns:**
java.util.Date - μια τιμή για ιδιότητες με τύπους ημερομηνίας (Date, Start, Finish).
### getDurationValue() {#getDurationValue--}
```
public final Duration getDurationValue()
```


Λαμβάνει την τιμή για ιδιότητες με τύπο 'Duration'.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - value for attributes with 'Duration' type.
### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Λαμβάνει το αναγνωριστικό ενός πεδίου.

**Returns:**
java.lang.String - το αναγνωριστικό ενός πεδίου.
### getFlagValue() {#getFlagValue--}
```
public final boolean getFlagValue()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα με τύπο 'Flag'.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα με τύπο 'Flag'.
### getNumericValue() {#getNumericValue--}
```
public final BigDecimal getNumericValue()
```


Λαμβάνει μια τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number).

**Returns:**
java.math.BigDecimal - μια τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number).
### getTextValue() {#getTextValue--}
```
public final String getTextValue()
```


Λαμβάνει μια τιμή για ιδιότητες με τύπο 'Text'.

**Returns:**
java.lang.String - μια τιμή για ιδιότητες με τύπο 'Text'.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Λαμβάνει το guid μιας τιμής αναζήτησης.

--------------------

Δεν πρέπει να ορίζεται απευθείας· αντί αυτού χρησιμοποιήστε ExtendedAttributeDefinition.CreateExtendedAttribute(Value lookupValue) για να δημιουργήσετε μια εκτεταμένη ιδιότητα με τιμή αναζήτησης.

**Returns:**
java.lang.String - το guid μιας τιμής αναζήτησης.
### getValueReadOnly() {#getValueReadOnly--}
```
public final boolean getValueReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν μια τιμή αυτού του αντικειμένου [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) είναι μόνο για ανάγνωση.

Value: επιστρέφει true εάν έχει οριστεί τύπος ή συγκέντρωση στο [ExtendedAttributeDefinition](../../com.aspose.tasks/extendedattributedefinition) για αυτό το αντικείμενο.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν μια τιμή αυτού του αντικειμένου [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) είναι μόνο για ανάγνωση.
### isErrorValue() {#isErrorValue--}
```
public final boolean isErrorValue()
```


Λαμβάνει εάν ο υπολογισμός της τιμής της εκτεταμένης ιδιότητας κατέληξε σε σφάλμα.

**Returns:**
boolean - εάν ο υπολογισμός της τιμής της εκτεταμένης ιδιότητας κατέληξε σε σφάλμα.
### setDateValue(Date value) {#setDateValue-java.util.Date-}
```
public final void setDateValue(Date value)
```


Ορίζει μια τιμή για ιδιότητες με τύπους ημερομηνίας (Date, Start, Finish).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | μια τιμή για ιδιότητες με τύπους ημερομηνίας (Date, Start, Finish). |

### setDurationValue(Duration value) {#setDurationValue-com.aspose.tasks.Duration-}
```
public final void setDurationValue(Duration value)
```


Ορίζει τιμή για ιδιότητες με τύπο 'Duration'.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Τιμή για ιδιότητες με τύπο 'Duration'. |

### setFlagValue(boolean value) {#setFlagValue-boolean-}
```
public final void setFlagValue(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για μια ιδιότητα με τύπο 'Flag'.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | Τιμή που υποδεικνύει αν έχει οριστεί σημαία για μια ιδιότητα τύπου 'Flag'. |

### setNumericValue(BigDecimal value) {#setNumericValue-java.math.BigDecimal-}
```
public final void setNumericValue(BigDecimal value)
```


Ορίζει μια τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.math.BigDecimal | Τιμή για ιδιότητες με αριθμητικούς τύπους (Cost, Number). |

### setTextValue(String value) {#setTextValue-java.lang.String-}
```
public final void setTextValue(String value)
```


Ορίζει μια τιμή για ιδιότητες με τύπο 'Text'.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Τιμή για ιδιότητες τύπου 'Text'. |

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς μιας εκτεταμένης ιδιότητας.

**Returns:**
java.lang.String - Η αναπαράσταση συμβολοσειράς της επεκταμένης ιδιότητας.

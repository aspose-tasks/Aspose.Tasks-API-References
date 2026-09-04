---
title: "PrimaveraSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera XER."
type: docs
weight: 208
url: /el/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera XER.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Λαμβάνει το βήμα αύξησης που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Λαμβάνει το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Λαμβάνει το επίθημα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Λαμβάνει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Ορίζει το βήμα αύξησης που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Ορίζει το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Ορίζει το επίθημα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των activity IDs. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Λαμβάνει το βήμα αύξησης που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Returns:**
int - η αύξηση που χρησιμοποιείται στην επανααρίθμηση των activity IDs.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Λαμβάνει το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Returns:**
java.lang.String - το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των activity IDs.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Λαμβάνει το επίθημα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Returns:**
int - το επίθημα που χρησιμοποιείται στην επανααρίθμηση των activity IDs.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των activity IDs.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή.

Το λογισμικό Primavera δεν υποστηρίζει εκχωρήσεις πόρων σε εργασίες σύνοψης (WBS). Έτσι, η εξαγωγή τέτοιων εκχωρήσεων μπορεί να οδηγήσει σε μη έγκυρο αρχείο σύμφωνα με το μοντέλο του Primavera. Εάν είναι true, οι εκχωρήσεις σε εργασίες σύνοψης παραλείπονται κατά την εξαγωγή. Εάν είναι false (η προεπιλεγμένη τιμή), θα εξαχθεί εξαίρεση εάν εντοπιστεί εκχώρηση σε εργασία σύνοψης κατά την εξαγωγή.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε εργασίες σύνοψης πρέπει να παραλείπονται κατά την εξαγωγή.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Ορίζει το βήμα αύξησης που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η αύξηση που χρησιμοποιείται στην επανααρίθμηση των activity IDs. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Ορίζει το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | το πρόθεμα που χρησιμοποιείται στην επανααρίθμηση των activity IDs. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Ορίζει το επίθημα που χρησιμοποιείται στην επανααρίθμηση των αναγνωριστικών δραστηριότητας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | το επίθημα που χρησιμοποιείται στην επανααρίθμηση των activity IDs. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των activity IDs.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν χρειάζεται η επανααρίθμηση των activity IDs. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή.

Το λογισμικό Primavera δεν υποστηρίζει εκχωρήσεις πόρων σε εργασίες σύνοψης (WBS). Έτσι, η εξαγωγή τέτοιων εκχωρήσεων μπορεί να οδηγήσει σε μη έγκυρο αρχείο σύμφωνα με το μοντέλο του Primavera. Εάν είναι true, οι εκχωρήσεις σε εργασίες σύνοψης παραλείπονται κατά την εξαγωγή. Εάν είναι false (η προεπιλεγμένη τιμή), θα εξαχθεί εξαίρεση εάν εντοπιστεί εκχώρηση σε εργασία σύνοψης κατά την εξαγωγή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε εργασίες σύνοψης πρέπει να παραλείπονται κατά την εξαγωγή. |


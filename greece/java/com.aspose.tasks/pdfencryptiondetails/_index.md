---
title: "PdfEncryptionDetails"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Περιέχει λεπτομέρειες για μια κρυπτογράφηση PDF."
type: docs
weight: 189
url: /el/java/com.aspose.tasks/pdfencryptiondetails/
---

**Inheritance:**
java.lang.Object
```
public class PdfEncryptionDetails
```

Περιέχει λεπτομέρειες για μια κρυπτογράφηση PDF.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)](#PdfEncryptionDetails-java.lang.String-java.lang.String-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getEncryptionAlgorithm()](#getEncryptionAlgorithm--) | Λαμβάνει τη λειτουργία κρυπτογράφησης. |
| [getOwnerPassword()](#getOwnerPassword--) | Λαμβάνει τον κωδικό πρόσβασης του Ιδιοκτήτη. |
| [getPermissions()](#getPermissions--) | Λαμβάνει τα δικαιώματα. |
| [getUserPassword()](#getUserPassword--) | Λαμβάνει τον κωδικό πρόσβασης του Χρήστη. |
| [setEncryptionAlgorithm(int value)](#setEncryptionAlgorithm-int-) | Ορίζει τη λειτουργία κρυπτογράφησης. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης του Ιδιοκτήτη. |
| [setPermissions(int value)](#setPermissions-int-) | Ορίζει τα δικαιώματα. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης του Χρήστη. |
### PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm) {#PdfEncryptionDetails-java.lang.String-java.lang.String-int-}
```
public PdfEncryptionDetails(String userPassword, String ownerPassword, int encryptionAlgorithm)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| userPassword | java.lang.String | Ο κωδικός πρόσβασης του χρήστη που επιτρέπει το άνοιγμα προστατευμένων εγγράφων. |
| ownerPassword | java.lang.String | Ο κωδικός πρόσβασης του ιδιοκτήτη που επιτρέπει το άνοιγμα προστατευμένων εγγράφων. |
| encryptionAlgorithm | int | Η παρουσία του [PdfEncryptionAlgorithm](../../com.aspose.tasks/pdfencryptionalgorithm) που υποδεικνύει τον αλγόριθμο κρυπτογράφησης. |

### getEncryptionAlgorithm() {#getEncryptionAlgorithm--}
```
public final int getEncryptionAlgorithm()
```


Λαμβάνει τη λειτουργία κρυπτογράφησης.

**Returns:**
int - η λειτουργία κρυπτογράφησης.
### getOwnerPassword() {#getOwnerPassword--}
```
public final String getOwnerPassword()
```


Λαμβάνει τον κωδικό πρόσβασης του Ιδιοκτήτη.

--------------------

Το άνοιγμα του εγγράφου με τον σωστό κωδικό πρόσβασης του ιδιοκτήτη (υποθέτοντας ότι δεν είναι ίδιος με τον κωδικό πρόσβασης του χρήστη) επιτρέπει πλήρη (ιδιοκτήτη) πρόσβαση στο έγγραφο. Αυτή η απεριόριστη πρόσβαση περιλαμβάνει τη δυνατότητα αλλαγής των κωδικών πρόσβασης του εγγράφου και των δικαιωμάτων πρόσβασης.

**Returns:**
java.lang.String - ο κωδικός πρόσβασης του Ιδιοκτήτη.
### getPermissions() {#getPermissions--}
```
public final int getPermissions()
```


Λαμβάνει τα δικαιώματα.

**Returns:**
int - τα δικαιώματα.
### getUserPassword() {#getUserPassword--}
```
public final String getUserPassword()
```


Λαμβάνει τον κωδικό πρόσβασης του Χρήστη.

--------------------

Το άνοιγμα του εγγράφου με τον σωστό κωδικό πρόσβασης του χρήστη (ή το άνοιγμα ενός εγγράφου που δεν έχει κωδικό πρόσβασης χρήστη) επιτρέπει την εκτέλεση πρόσθετων λειτουργιών σύμφωνα με τα δικαιώματα πρόσβασης του χρήστη που καθορίζονται στο λεξικό κρυπτογράφησης του εγγράφου.

**Returns:**
java.lang.String - ο κωδικός χρήστη.
### setEncryptionAlgorithm(int value) {#setEncryptionAlgorithm-int-}
```
public final void setEncryptionAlgorithm(int value)
```


Ορίζει τη λειτουργία κρυπτογράφησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η λειτουργία κρυπτογράφησης. |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public final void setOwnerPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης του Ιδιοκτήτη.

--------------------

Το άνοιγμα του εγγράφου με τον σωστό κωδικό πρόσβασης του ιδιοκτήτη (υποθέτοντας ότι δεν είναι ίδιος με τον κωδικό πρόσβασης του χρήστη) επιτρέπει πλήρη (ιδιοκτήτη) πρόσβαση στο έγγραφο. Αυτή η απεριόριστη πρόσβαση περιλαμβάνει τη δυνατότητα αλλαγής των κωδικών πρόσβασης του εγγράφου και των δικαιωμάτων πρόσβασης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ο κωδικός ιδιοκτήτη. |

### setPermissions(int value) {#setPermissions-int-}
```
public final void setPermissions(int value)
```


Ορίζει τα δικαιώματα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | τα δικαιώματα. |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public final void setUserPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης του Χρήστη.

--------------------

Το άνοιγμα του εγγράφου με τον σωστό κωδικό πρόσβασης του χρήστη (ή το άνοιγμα ενός εγγράφου που δεν έχει κωδικό πρόσβασης χρήστη) επιτρέπει την εκτέλεση πρόσθετων λειτουργιών σύμφωνα με τα δικαιώματα πρόσβασης του χρήστη που καθορίζονται στο λεξικό κρυπτογράφησης του εγγράφου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | ο κωδικός χρήστη. |


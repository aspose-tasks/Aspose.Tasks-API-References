---
title: "ProjectServerSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών όταν το έργο αποθηκεύεται στο Project Server ή στο Project Online."
type: docs
weight: 227
url: /el/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών όταν το έργο αποθηκεύεται στο Project Server ή στο Project Online.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Λαμβάνει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά. |
| [getProjectGuid()](#getProjectGuid--) | Λαμβάνει το μοναδικό αναγνωριστικό ενός έργου. |
| [getProjectName()](#getProjectName--) | Λαμβάνει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online. |
| [getTimeout()](#getTimeout--) | Λαμβάνει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας της αίτησης αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Ορίζει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Ορίζει το μοναδικό αναγνωριστικό ενός έργου. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Ορίζει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | Ορίζει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας της αίτησης αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Λαμβάνει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά. Η προεπιλεγμένη τιμή είναι 2 δευτερόλεπτα.

**Returns:**
double - διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Λαμβάνει το μοναδικό αναγνωριστικό ενός έργου. Θα πρέπει να είναι μοναδικό εντός του Project Server \\ Project Online.

**Returns:**
java.util.UUID - μοναδικό αναγνωριστικό ενός έργου.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Λαμβάνει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online. Θα πρέπει να είναι μοναδικό εντός του Project Server \\ Project Online. Εάν η τιμή παραλειφθεί, θα χρησιμοποιηθεί η τιμή της ιδιότητας Prj.Name.

**Returns:**
java.lang.String - όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Λαμβάνει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας της αίτησης αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. Η προεπιλεγμένη τιμή για αυτήν την ιδιότητα είναι 1 λεπτό.

--------------------

Ο χρόνος επεξεργασίας μπορεί να είναι μεγαλύτερος για μεγάλα έργα ή σε περίπτωση που το στιγμιότυπο του Project Server είναι πολύ απασχολημένο να απαντά σε άλλα αιτήματα.

**Returns:**
double - χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Ορίζει το διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά. Η προεπιλεγμένη τιμή είναι 2 δευτερόλεπτα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | διάστημα μεταξύ των αιτήσεων κατάστασης εργασιών στην ουρά. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Ορίζει το μοναδικό αναγνωριστικό ενός έργου. Θα πρέπει να είναι μοναδικό εντός του στιγμιότυπου του Project Server \\ Project Online.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.UUID | μοναδικό αναγνωριστικό ενός έργου. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Ορίζει το όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online. Θα πρέπει να είναι μοναδικό εντός του στιγμιότυπου του Project Server \\ Project Online. Εάν η τιμή παραλειφθεί, θα χρησιμοποιηθεί η τιμή της ιδιότητας Prj.Name.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | όνομα ενός έργου που εμφανίζεται στη λίστα έργων του Project Server \\ Project Online. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Ορίζει το χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. Η προεπιλεγμένη τιμή για αυτήν την ιδιότητα είναι 1 λεπτό.

--------------------

Ο χρόνος επεξεργασίας μπορεί να είναι μεγαλύτερος για μεγάλα έργα ή σε περίπτωση που το στιγμιότυπο του Project Server είναι πολύ απασχολημένο να απαντά σε άλλα αιτήματα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | double | χρονικό όριο που χρησιμοποιείται κατά την αναμονή επεξεργασίας του αιτήματος αποθήκευσης έργου από την υπηρεσία επεξεργασίας ουράς του Project Server. |


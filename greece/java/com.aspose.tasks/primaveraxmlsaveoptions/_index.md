---
title: "PrimaveraXmlSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera xml."
type: docs
weight: 212
url: /el/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του έργου σε μορφή Primavera xml.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα αποθηκευτεί μια ριζική εργασία ή όχι. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα αποθηκευτεί μια ριζική εργασία ή όχι. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions).

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα αποθηκευτεί μια ριζική εργασία ή όχι.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν θα αποθηκευτεί μια ρίζα εργασίας ή όχι.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι εκχωρήσεις πόρων σε συνοπτικές εργασίες πρέπει να παραλειφθούν κατά την εξαγωγή.

Το λογισμικό Primavera δεν υποστηρίζει εκχωρήσεις πόρων σε εργασίες σύνοψης (WBS). Έτσι, η εξαγωγή τέτοιων εκχωρήσεων μπορεί να οδηγήσει σε μη έγκυρο αρχείο σύμφωνα με το μοντέλο του Primavera. Εάν είναι true, οι εκχωρήσεις σε εργασίες σύνοψης παραλείπονται κατά την εξαγωγή. Εάν είναι false (η προεπιλεγμένη τιμή), θα εξαχθεί εξαίρεση εάν εντοπιστεί εκχώρηση σε εργασία σύνοψης κατά την εξαγωγή.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν οι εκχωρήσεις πόρων σε εργασίες σύνοψης πρέπει να παραλείπονται κατά την εξαγωγή.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα αποθηκευτεί μια ριζική εργασία ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει αν θα αποθηκευτεί μια ρίζα εργασίας ή όχι. |

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


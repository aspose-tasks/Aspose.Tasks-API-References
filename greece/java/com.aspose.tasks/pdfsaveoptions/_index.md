---
title: "PdfSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων έργου σε PDF."
type: docs
weight: 191
url: /el/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων έργου σε PDF.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση ενός εγγράφου στη μορφή [SaveFileFormat](../../com.aspose/tasks/savefileformat). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \\{@inheritDoc\\} |
| [deepClone()](#deepClone--) | \\{@inheritDoc\\} |
| [getCompliance()](#getCompliance--) | Λαμβάνει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Λαμβάνει λεπτομέρειες κρυπτογράφησης. |
| [getFontSettings()](#getFontSettings--) | Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Λαμβάνει μια κλήση επιστροφής ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [getPages()](#getPages--) | Λαμβάνει τη λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία. |
| [getTextCompression()](#getTextCompression--) | Λαμβάνει έναν τύπο συμπίεσης που θα χρησιμοποιηθεί για όλα τα ρεύματα περιεχομένου εκτός των εικόνων. |
| [setCompliance(int value)](#setCompliance-int-) | Ορίζει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Ορίζει λεπτομέρειες κρυπτογράφησης. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ορίζει μια κλήση επιστροφής που ορίζεται από τον χρήστη και χρησιμοποιείται για τη λήψη ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ορίζει τη λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία. |
| [setTextCompression(int value)](#setTextCompression-int-) | Ορίζει έναν τύπο συμπίεσης που θα χρησιμοποιηθεί για όλα τα ρεύματα περιεχομένου εκτός των εικόνων. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PdfSaveOptions](../../com.aspose/tasks/pdfsaveoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση ενός εγγράφου στη μορφή [SaveFileFormat](../../com.aspose/tasks/savefileformat).

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Δεσμευμένο για εσωτερική χρήση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \\{@inheritDoc\\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Δεσμευμένο για εσωτερική χρήση.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Λαμβάνει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. Η προεπιλογή είναι [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\\#Pdf15).

**Returns:**
int - ένα επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Λαμβάνει λεπτομέρειες κρυπτογράφησης. Εάν δεν οριστεί, δεν θα γίνει καμία κρυπτογράφηση.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Λαμβάνει μια καθορισμένη από τον χρήστη κλήση επιστροφής που χρησιμοποιείται για την απόκτηση μιας ροής εξόδου για κάθε αποδομένη σελίδα. Ισχύει όταν χρησιμοποιείται η επιλογή `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\\#setSaveToSeparateFiles-boolean-)).

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Λαμβάνει τη λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.

--------------------

Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - η λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Returns:**
boolean - τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Λαμβάνει έναν τύπο συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από εικόνες. Η προεπιλογή είναι [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Returns:**
int - ένας τύπος συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από εικόνες.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Ορίζει το επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. Η προεπιλογή είναι [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένα επιθυμητό επίπεδο συμμόρφωσης για το παραγόμενο έγγραφο PDF. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Ορίζει λεπτομέρειες κρυπτογράφησης. Εάν δεν οριστεί, τότε δεν θα εκτελεστεί κρυπτογράφηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | λεπτομέρειες κρυπτογράφησης. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ορίζει μια κλήση επιστροφής καθορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. Ισχύει όταν η επιλογή `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) χρησιμοποιείται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | μια callback ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Ορίζει τη λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.

--------------------

Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;java.lang.Integer&gt; | η λίστα των αριθμών σελίδων που θα αποθηκευτούν όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα αποθηκευτούν οι σελίδες του έργου σε ξεχωριστά αρχεία. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Ορίζει έναν τύπο συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από εικόνες. Η προεπιλογή είναι [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ένας τύπος συμπίεσης που θα χρησιμοποιηθεί για όλες τις ροές περιεχομένου εκτός από εικόνες. |


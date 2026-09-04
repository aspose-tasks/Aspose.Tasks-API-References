---
title: "ImageSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε εικόνες."
type: docs
weight: 134
url: /el/java/com.aspose.tasks/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class ImageSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε εικόνες.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ImageSaveOptions(int saveFormat)](#ImageSaveOptions-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ImageSaveOptions](../../com.aspose/tasks/imagesaveoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση αποδιδόμενων εικόνων σε μορφές TIFF, PNG, BMP ή JPEG. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \\{@inheritDoc\\} |
| [deepClone()](#deepClone--) | \\{@inheritDoc\\} |
| [getFontSettings()](#getFontSettings--) | Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Λαμβάνει την οριζόντια ανάλυση σε dpi. |
| [getJpegQuality()](#getJpegQuality--) | Λαμβάνει μια ποιότητα JPEG. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Λαμβάνει μια κλήση επιστροφής ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [getPages()](#getPages--) | Λαμβάνει μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |
| [getPixelFormat()](#getPixelFormat--) | Λαμβάνει τη μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [getTiffCompression()](#getTiffCompression--) | Λαμβάνει τον τύπο συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες στη μορφή TIFF. |
| [getVerticalResolution()](#getVerticalResolution--) | Λαμβάνει την κάθετη ανάλυση σε dpi. |
| [setHorizontalResolution(float value)](#setHorizontalResolution-float-) | Ορίζει την οριζόντια ανάλυση σε dpi. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Ορίζει μια ποιότητα JPEG. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ορίζει μια κλήση επιστροφής που ορίζεται από τον χρήστη και χρησιμοποιείται για τη λήψη ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ορίζει μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |
| [setPixelFormat(int value)](#setPixelFormat-int-) | Ορίζει τη μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Ορίζει τον τύπο συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες στη μορφή TIFF. |
| [setVerticalResolution(float value)](#setVerticalResolution-float-) | Ορίζει την κάθετη ανάλυση σε dpi. |
### ImageSaveOptions(int saveFormat) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int saveFormat)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ImageSaveOptions](../../com.aspose/tasks/imagesaveoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση αποδιδόμενων εικόνων σε μορφές TIFF, PNG, BMP ή JPEG.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| saveFormat | int | Μπορεί να είναι TIFF, PNG, BMP ή JPEG[SaveFileFormat](../../com.aspose.tasks/savefileformat). |

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public final void copyOutputPropertiesFrom(SaveOptions source)
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
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getHorizontalResolution() {#getHorizontalResolution--}
```
public final float getHorizontalResolution()
```


Λαμβάνει την οριζόντια ανάλυση σε dpi.

**Returns:**
float - η οριζόντια ανάλυση σε dpi.
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Λαμβάνει μια ποιότητα JPEG. Η επιτρεπόμενη περιοχή τιμών είναι 0..100.

**Returns:**
int - μια ποιότητα JPEG.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Λαμβάνει μια κλήση επιστροφής ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Λαμβάνει μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.

--------------------

Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.
### getPixelFormat() {#getPixelFormat--}
```
public final int getPixelFormat()
```


Λαμβάνει τη μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα.

**Returns:**
int - η μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Returns:**
boolean - τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Λαμβάνει τον τύπο συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες στη μορφή TIFF.

--------------------

Έχει επίδραση μόνο όταν αποθηκεύεται σε TIFF. Η προεπιλεγμένη τιμή είναι `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Returns:**
int - ο τύπος συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες στη μορφή TIFF.
### getVerticalResolution() {#getVerticalResolution--}
```
public final float getVerticalResolution()
```


Λαμβάνει την κάθετη ανάλυση σε dpi.

**Returns:**
float - η κάθετη ανάλυση σε dpi.
### setHorizontalResolution(float value) {#setHorizontalResolution-float-}
```
public final void setHorizontalResolution(float value)
```


Ορίζει την οριζόντια ανάλυση σε dpi.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | η οριζόντια ανάλυση σε dpi. |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Ορίζει την ποιότητα JPEG. Η επιτρεπόμενη περιοχή τιμών είναι 0..100.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | μια ποιότητα JPEG. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ορίζει μια κλήση επιστροφής που ορίζεται από τον χρήστη και χρησιμοποιείται για τη λήψη ροής εξόδου για κάθε αποδοθείσα σελίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | μια callback ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Ορίζει μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία.

--------------------

Όλες οι σελίδες θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;java.lang.Integer&gt; | μια λίστα αριθμών σελίδων για αποθήκευση όταν αποθηκεύεται η διάταξη του έργου σε ξεχωριστά αρχεία. |

### setPixelFormat(int value) {#setPixelFormat-int-}
```
public final void setPixelFormat(int value)
```


Ορίζει τη μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | η μορφή των δεδομένων χρώματος για κάθε pixel στην εικόνα. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Ορίζει τον τύπο συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες στη μορφή TIFF.

--------------------

Έχει επίδραση μόνο όταν αποθηκεύεται σε TIFF. Η προεπιλεγμένη τιμή είναι `TiffCompressionLZW`([getTiffCompression()](../../com.aspose.tasks/imagesaveoptions\#getTiffCompression--)/[setTiffCompression(int)](../../com.aspose.tasks/imagesaveoptions\#setTiffCompression-int-)).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τύπος συμπίεσης που θα εφαρμοστεί όταν αποθηκεύονται οι παραγόμενες εικόνες σε μορφή TIFF. |

### setVerticalResolution(float value) {#setVerticalResolution-float-}
```
public final void setVerticalResolution(float value)
```


Ορίζει την κάθετη ανάλυση σε dpi.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | η κάθετη ανάλυση σε dpi. |


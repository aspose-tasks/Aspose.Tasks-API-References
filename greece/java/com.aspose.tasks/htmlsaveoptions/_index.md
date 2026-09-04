---
title: "HtmlSaveOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε HTML."
type: docs
weight: 132
url: /el/java/com.aspose.tasks/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class HtmlSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε HTML.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) class. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \\{@inheritDoc\\} |
| [deepClone()](#deepClone--) | \\{@inheritDoc\\} |
| [getCssSavingCallback()](#getCssSavingCallback--) | Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης CSS. |
| [getCssStylePrefix()](#getCssStylePrefix--) | Λαμβάνει το πρόθεμα στυλ CSS. |
| [getExportCss()](#getExportCss--) | Λαμβάνει τον τρόπο εξαγωγής του CSS. |
| [getExportFonts()](#getExportFonts--) | Λαμβάνει τον τρόπο εξαγωγής των γραμματοσειρών. |
| [getExportImages()](#getExportImages--) | Λαμβάνει τον τρόπο εξαγωγής των εικόνων. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Λαμβάνει τους τύπους γραμματοσειρών. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς. |
| [getFontSettings()](#getFontSettings--) | Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς. |
| [getIncludeProjectNameInPageHeader()](#getIncludeProjectNameInPageHeader--) | Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML. |
| [getIncludeProjectNameInTitle()](#getIncludeProjectNameInTitle--) | Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Λαμβάνει μια κλήση επιστροφής ορισμένη από τον χρήστη που χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [getPages()](#getPages--) | Λαμβάνει μια λίστα αριθμών σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Λαμβάνει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-) | Ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης CSS. |
| [setCssStylePrefix(String value)](#setCssStylePrefix-java.lang.String-) | Ορίζει το πρόθεμα στυλ CSS. |
| [setExportCss(int value)](#setExportCss-int-) | Ορίζει τον τρόπο εξαγωγής του CSS. |
| [setExportFonts(int value)](#setExportFonts-int-) | Ορίζει τον τρόπο εξαγωγής των γραμματοσειρών. |
| [setExportImages(int value)](#setExportImages-int-) | Ορίζει τον τρόπο εξαγωγής των εικόνων. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Ορίζει τους τύπους γραμματοσειρών. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-) | Ορίζει την κλήση επιστροφής (callback) που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-) | Ορίζει την κλήση επιστροφής (callback) που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς. |
| [setIncludeProjectNameInPageHeader(boolean value)](#setIncludeProjectNameInPageHeader-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML. |
| [setIncludeProjectNameInTitle(boolean value)](#setIncludeProjectNameInTitle-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ορίζει μια κλήση επιστροφής που ορίζεται από τον χρήστη και χρησιμοποιείται για τη λήψη ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Ορίζει μια λίστα αριθμών σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HtmlSaveOptions](../../com.aspose.tasks/htmlsaveoptions) class.

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
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) - the callback that is called to create resource to store CSS.
### getCssStylePrefix() {#getCssStylePrefix--}
```
public final String getCssStylePrefix()
```


Λαμβάνει το πρόθεμα στυλ CSS.

**Returns:**
java.lang.String - πρόθεμα στυλ CSS.
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Λαμβάνει τον τρόπο εξαγωγής του CSS.

**Returns:**
int - ο τρόπος εξαγωγής του CSS.
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Λαμβάνει τον τρόπο εξαγωγής των γραμματοσειρών.

**Returns:**
int - ο τρόπος εξαγωγής των γραμματοσειρών.
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Λαμβάνει τον τρόπο εξαγωγής των εικόνων.

**Returns:**
int - ο τρόπος εξαγωγής των εικόνων.
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Λαμβάνει τους τύπους γραμματοσειρών.

Τιμή: Οι τύποι γραμματοσειρών.

**Returns:**
int - οι τύποι γραμματοσειρών.
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς.

**Returns:**
[IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) - the callback that is called to create resource to store font.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Λαμβάνει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς.

**Returns:**
[IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) - the callback that is called to create resource to store font.
### getIncludeProjectNameInPageHeader() {#getIncludeProjectNameInPageHeader--}
```
public final boolean getIncludeProjectNameInPageHeader()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML.
### getIncludeProjectNameInTitle() {#getIncludeProjectNameInTitle--}
```
public final boolean getIncludeProjectNameInTitle()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML.
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


Λαμβάνει μια λίστα αριθμών σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου.

--------------------

Όλες οι σελίδες του έργου θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - λίστα αριθμών σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Λαμβάνει μια τιμή που υποδεικνύει αν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Returns:**
boolean - τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Λαμβάνει μια τιμή που υποδεικνύει αν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου.

--------------------

Η τρέχουσα χρήση διαβαθμισμένου πινέλου δεν υποστηρίζεται κατά την απόδοση σε HTML.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου.
### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.tasks.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης CSS.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.tasks/icsssavingcallback) | η κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης του CSS. |

### setCssStylePrefix(String value) {#setCssStylePrefix-java.lang.String-}
```
public final void setCssStylePrefix(String value)
```


Ορίζει το πρόθεμα στυλ CSS.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Πρόθεμα στυλ CSS. |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Ορίζει τον τρόπο εξαγωγής του CSS.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τρόπος εξαγωγής των CSS. |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Ορίζει τον τρόπο εξαγωγής των γραμματοσειρών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τρόπος εξαγωγής των γραμματοσειρών. |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Ορίζει τον τρόπο εξαγωγής των εικόνων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ο τρόπος εξαγωγής των εικόνων. |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Ορίζει τους τύπους γραμματοσειρών.

Τιμή: Οι τύποι γραμματοσειρών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | οι τύποι γραμματοσειρών. |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.tasks.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Ορίζει την κλήση επιστροφής (callback) που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.tasks/ifontsavingcallback) | η callback που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς. |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.tasks.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Ορίζει την κλήση επιστροφής (callback) που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.tasks/iimagesavingcallback) | η callback που καλείται για τη δημιουργία πόρου αποθήκευσης γραμματοσειράς. |

### setIncludeProjectNameInPageHeader(boolean value) {#setIncludeProjectNameInPageHeader-boolean-}
```
public final void setIncludeProjectNameInPageHeader(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στην κεφαλίδα της σελίδας HTML. |

### setIncludeProjectNameInTitle(boolean value) {#setIncludeProjectNameInTitle-boolean-}
```
public final void setIncludeProjectNameInTitle(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα συμπεριληφθεί το όνομα του έργου στον τίτλο HTML. |

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


Ορίζει μια λίστα αριθμών σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου.

--------------------

Όλες οι σελίδες του έργου θα αποθηκευτούν εάν αυτή η λίστα είναι κενή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.List&lt;java.lang.Integer&gt; | μια λίστα με αριθμούς σελίδων για αποθήκευση κατά την απόδοση της διάταξης του έργου. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν πρέπει να μειωθεί το κενό μεταξύ της τελευταίας εργασίας και του υποσέλιδου. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί διαβαθμισμένο πινέλο κατά την απόδοση της διάταξης του έργου.

--------------------

Η τρέχουσα χρήση διαβαθμισμένου πινέλου δεν υποστηρίζεται κατά την απόδοση σε HTML.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί πινέλο διαβάθμισης κατά την απόδοση της διάταξης του έργου. |


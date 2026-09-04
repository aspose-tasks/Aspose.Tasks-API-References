---
title: "SvgOptions"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε SVG."
type: docs
weight: 283
url: /el/java/com.aspose.tasks/svgoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.ICloneableSaveOptions
```
public class SvgOptions extends SaveOptions implements ICloneableSaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του έργου σε SVG.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SvgOptions()](#SvgOptions--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [SvgOptions](../../com.aspose.tasks/svgoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή SVG. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \\{@inheritDoc\\} |
| [deepClone()](#deepClone--) | \\{@inheritDoc\\} |
| [getPageSavingCallback()](#getPageSavingCallback--) | Λαμβάνει μια callback υλοποίησης που ορίζεται από τον χρήστη και χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Ορίζει μια callback υλοποίησης που ορίζεται από τον χρήστη και χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. |
### SvgOptions() {#SvgOptions--}
```
public SvgOptions()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [SvgOptions](../../com.aspose.tasks/svgoptions) που μπορεί να χρησιμοποιηθεί για την αποθήκευση του έργου σε μορφή SVG.

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
public final SaveOptions deepClone()
```


Δεσμευμένο για εσωτερική χρήση.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Λαμβάνει μια callback υλοποίησης που ορίζεται από τον χρήστη και χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined implementation callback which is used to get an output stream for each rendered page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου.

--------------------

Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου.
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Ορίζει μια callback υλοποίησης που ορίζεται από τον χρήστη και χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | μια callback υλοποίησης που ορίζεται από τον χρήστη και χρησιμοποιείται για την απόκτηση ροής εξόδου για κάθε αποδοθείσα σελίδα. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Καθορίζει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου.

--------------------

Προς το παρόν η χρήση του gradient brush δεν υποστηρίζεται για απόδοση σε SVG.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα χρησιμοποιηθεί gradient brush κατά την απόδοση της διάταξης του έργου. |


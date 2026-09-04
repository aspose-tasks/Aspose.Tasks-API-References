---
title: "FontSettings"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής έργων."
type: docs
weight: 101
url: /el/java/com.aspose.tasks/fontsettings/
---

**Inheritance:**
java.lang.Object
```
public final class FontSettings
```

Καθορίζει τις ρυθμίσεις γραμματοσειράς που χρησιμοποιούνται κατά την απόδοση της προβολής του έργου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FontSettings()](#FontSettings--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDefaultFontName()](#getDefaultFontName--) | Λαμβάνει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση. |
| [getFontResolveCallback()](#getFontResolveCallback--) | Λαμβάνει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών. |
| [getUseProjectDefaultFont()](#getUseProjectDefaultFont--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιηθεί για την απόδοση. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση. |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ορίζει τους φακέλους όπου το Aspose.Tasks αναζητά γραμματοσειρές TrueType κατά την απόδοση της προβολής του έργου. |
| [setFontResolveCallback(FontResolveCallbackDelegate value)](#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-) | Ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών. |
| [setUseProjectDefaultFont(boolean value)](#setUseProjectDefaultFont-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιηθεί για την απόδοση. |
### FontSettings() {#FontSettings--}
```
public FontSettings()
```


### getDefaultFontName() {#getDefaultFontName--}
```
public final String getDefaultFontName()
```


Λαμβάνει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

**Returns:**
java.lang.String - η προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.
### getFontResolveCallback() {#getFontResolveCallback--}
```
public final FontResolveCallbackDelegate getFontResolveCallback()
```


Λαμβάνει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών.

**Returns:**
[FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) - a callback which can be used to customize resolved fonts.
### getUseProjectDefaultFont() {#getUseProjectDefaultFont--}
```
public final boolean getUseProjectDefaultFont()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιηθεί για την απόδοση.

--------------------

Όταν η τιμή είναι False και έχει οριστεί το DefaultFontName, η μηχανή απόδοσης θα χρησιμοποιήσει τη γραμματοσειρά που καθορίζεται από το DefaultFontName ως εφεδρική γραμματοσειρά. Διαφορετικά, χρησιμοποιούνται οι γραμματοσειρές 'Arial' (αν είναι εγκατεστημένη) ή 'Generic Sans Serif' ως εφεδρική γραμματοσειρά. Η εφεδρική γραμματοσειρά χρησιμοποιείται κατά την απόδοση της προβολής του έργου όταν ένα στυλ κειμένου αναφέρεται σε γραμματοσειρά που δεν είναι εγκατεστημένη στο τρέχον λειτουργικό σύστημα. Για μεγαλύτερο έλεγχο της επίλυσης γραμματοσειρών, μπορείτε να χρησιμοποιήσετε το `FontResolveCallback`([getFontResolveCallback](../../com.aspose/tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose/tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Returns:**
boolean - τιμή που υποδεικνύει εάν πρέπει να χρησιμοποιηθεί η προεπιλεγμένη γραμματοσειρά για την απόδοση.
### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public final void setDefaultFontName(String value)
```


Ορίζει την προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | η προεπιλεγμένη (ή εφεδρική) γραμματοσειρά για την απόδοση. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public final void setFontFolders(String[] fontFolders, boolean recursive)
```


Ορίζει τους φακέλους όπου το Aspose.Tasks αναζητά γραμματοσειρές TrueType κατά την απόδοση της προβολής του έργου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Ένας πίνακας φακέλων που περιέχουν γραμματοσειρές TrueType. |
| αναδρομικά | boolean | Εάν είναι true, οι καθορισμένοι φάκελοι θα σαρώνονται αναδρομικά. |

### setFontResolveCallback(FontResolveCallbackDelegate value) {#setFontResolveCallback-com.aspose.tasks.FontResolveCallbackDelegate-}
```
public final void setFontResolveCallback(FontResolveCallbackDelegate value)
```


Ορίζει μια κλήση επιστροφής που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [FontResolveCallbackDelegate](../../com.aspose.tasks/fontresolvecallbackdelegate) | μια callback που μπορεί να χρησιμοποιηθεί για την προσαρμογή των επιλυμένων γραμματοσειρών. |

### setUseProjectDefaultFont(boolean value) {#setUseProjectDefaultFont-boolean-}
```
public final void setUseProjectDefaultFont(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η προεπιλεγμένη γραμματοσειρά πρέπει να χρησιμοποιηθεί για την απόδοση.

--------------------

Όταν η τιμή είναι False και έχει οριστεί το DefaultFontName, η μηχανή απόδοσης θα χρησιμοποιήσει τη γραμματοσειρά που καθορίζεται από το DefaultFontName ως εφεδρική γραμματοσειρά. Διαφορετικά, χρησιμοποιούνται οι γραμματοσειρές 'Arial' (αν είναι εγκατεστημένη) ή 'Generic Sans Serif' ως εφεδρική γραμματοσειρά. Η εφεδρική γραμματοσειρά χρησιμοποιείται κατά την απόδοση της προβολής του έργου όταν ένα στυλ κειμένου αναφέρεται σε γραμματοσειρά που δεν είναι εγκατεστημένη στο τρέχον λειτουργικό σύστημα. Για μεγαλύτερο έλεγχο της επίλυσης γραμματοσειρών, μπορείτε να χρησιμοποιήσετε το `FontResolveCallback`([getFontResolveCallback](../../com.aspose/tasks/fontsettings\#getFontResolveCallback--)/[setFontResolveCallback(FontResolveCallbackDelegate)](../../com.aspose/tasks/fontsettings\#setFontResolveCallback-FontResolveCallbackDelegate-)) callback.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | μια τιμή που υποδεικνύει εάν πρέπει να χρησιμοποιηθεί η προεπιλεγμένη γραμματοσειρά για την απόδοση. |


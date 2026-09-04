---
title: "UsageView"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια προβολή χρήσης σε ένα έργο."
type: docs
weight: 331
url: /el/java/com.aspose.tasks/usageview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public abstract class UsageView extends View implements ITimescaledView
```

Αναπαριστά μια προβολή χρήσης σε ένα έργο.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAlignDetailsData()](#getAlignDetailsData--) | Λαμβάνει την ευθυγράμμιση δεδομένων λεπτομερειών. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του κάτω επιπέδου κλίμακας χρόνου της προβολής. |
| [getDisplayDetailsHeaderColumn()](#getDisplayDetailsHeaderColumn--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι. |
| [getDisplayShortDetailHeaderNames()](#getDisplayShortDetailHeaderNames--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του μεσαίου επιπέδου κλίμακας χρόνου της προβολής. |
| [getRepeatDetailsHeaderOnAllRows()](#getRepeatDetailsHeaderOnAllRows--) | Λαμβάνει μια τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \\{@inheritDoc\\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Λαμβάνει τις ρυθμίσεις του άνω επιπέδου κλίμακας χρόνου της προβολής. |
| [setAlignDetailsData(int value)](#setAlignDetailsData-int-) | Ορίζει την ευθυγράμμιση δεδομένων λεπτομερειών. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του κάτω επιπέδου κλίμακας χρόνου της προβολής. |
| [setDisplayDetailsHeaderColumn(boolean value)](#setDisplayDetailsHeaderColumn-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι. |
| [setDisplayShortDetailHeaderNames(boolean value)](#setDisplayShortDetailHeaderNames-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. |
| [setRepeatDetailsHeaderOnAllRows(boolean value)](#setRepeatDetailsHeaderOnAllRows-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \\{@inheritDoc\\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Ορίζει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. |
### getAlignDetailsData() {#getAlignDetailsData--}
```
public final int getAlignDetailsData()
```


Λαμβάνει την ευθυγράμμιση δεδομένων λεπτομερειών.

**Returns:**
int - ευθυγράμμιση δεδομένων λεπτομερειών.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getDisplayDetailsHeaderColumn() {#getDisplayDetailsHeaderColumn--}
```
public final boolean getDisplayDetailsHeaderColumn()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι.
### getDisplayShortDetailHeaderNames() {#getDisplayShortDetailHeaderNames--}
```
public final boolean getDisplayShortDetailHeaderNames()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getRepeatDetailsHeaderOnAllRows() {#getRepeatDetailsHeaderOnAllRows--}
```
public final boolean getRepeatDetailsHeaderOnAllRows()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Λαμβάνει ένα ποσοστό για τη μείωση ή την αύξηση του διαστήματος μεταξύ των μονάδων στο επίπεδο χρονοσειράς.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Λαμβάνει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setAlignDetailsData(int value) {#setAlignDetailsData-int-}
```
public final void setAlignDetailsData(int value)
```


Ορίζει την ευθυγράμμιση δεδομένων λεπτομερειών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | ευθυγράμμιση δεδομένων λεπτομερειών. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του κατώτερου επιπέδου χρονοσειράς της προβολής. |

### setDisplayDetailsHeaderColumn(boolean value) {#setDisplayDetailsHeaderColumn-boolean-}
```
public final void setDisplayDetailsHeaderColumn(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα εμφανίζεται η στήλη κεφαλίδας λεπτομερειών στην προβολή ή όχι. |

### setDisplayShortDetailHeaderNames(boolean value) {#setDisplayShortDetailHeaderNames-boolean-}
```
public final void setDisplayShortDetailHeaderNames(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα εμφανίζονται σύντομα ονόματα κεφαλίδας λεπτομερειών ή όχι. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του ενδιάμεσου επιπέδου χρονοσειράς της προβολής. |

### setRepeatDetailsHeaderOnAllRows(boolean value) {#setRepeatDetailsHeaderOnAllRows-boolean-}
```
public final void setRepeatDetailsHeaderOnAllRows(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | τιμή που υποδεικνύει εάν θα επαναλαμβάνεται η κεφαλίδα λεπτομερειών σε όλες τις γραμμές ανάθεσης ή όχι. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Ορίζει ένα ποσοστό για τη μείωση ή την αύξηση του διαστήματος μεταξύ των μονάδων στο επίπεδο χρονοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | \\{@inheritDoc\\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Ορίζει τις ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | ρυθμίσεις του ανώτερου επιπέδου χρονοσειράς της προβολής. |


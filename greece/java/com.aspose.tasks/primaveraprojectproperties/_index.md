---
title: "PrimaveraProjectProperties"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά ιδιότητες ειδικές για Primavera για ένα έργο που διαβάζεται από αρχεία Primavera XER ή P6XML."
type: docs
weight: 205
url: /el/java/com.aspose.tasks/primaveraprojectproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraProjectProperties
```

Αναπαριστά ιδιότητες ειδικές για Primavera για ένα έργο που διαβάστηκε από αρχεία Primavera (XER ή P6XML).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBaselineProjects()](#getBaselineProjects--) | Λαμβάνει τον πίνακα των βασικών έργων του τρέχοντος έργου. |
| [getCriticalActivitiesDefiningMethod()](#getCriticalActivitiesDefiningMethod--) | Λαμβάνει τη μέθοδο για τον ορισμό κρίσιμων δραστηριοτήτων: Longest Path ή Total Float. |
| [getCriticalTotalFloatLimit()](#getCriticalTotalFloatLimit--) | Λαμβάνει την τιμή κατωφλίου που χρησιμοποιείται για τον ορισμό κρίσιμων δραστηριοτήτων εάν χρησιμοποιείται η μέθοδος TotalFloat. |
| [getCurrentBaselineProjectId()](#getCurrentBaselineProjectId--) | Λαμβάνει το Id του τρέχοντος βασικού έργου. |
| [getIgnoreOtherProjectRelationships()](#getIgnoreOtherProjectRelationships--) | Λαμβάνει μια σημαία που καθορίζει εάν θα αγνοηθούν οι σχέσεις δραστηριοτήτων μεταξύ έργων. |
| [getMakeOpenEndedActivitiesCritical()](#getMakeOpenEndedActivitiesCritical--) | Λαμβάνει μια σημαία που καθορίζει εάν οι δραστηριότητες πρέπει να σημειωθούν ως κρίσιμες κατά τον προγραμματισμό του έργου. |
| [getRelationshipLagCalendar()](#getRelationshipLagCalendar--) | Λαμβάνει μια επιλογή που καθορίζει ποιο ημερολόγιο θα χρησιμοποιηθεί για τον προγραμματισμό του καθυστέρησης σχέσης (Relationship Lag) σε έργα Primavera. |
| [getShortName()](#getShortName--) | Λαμβάνει το σύντομο όνομα του έργου (Αναγνωριστικό έργου). |
| [getUseExpectedFinishDates()](#getUseExpectedFinishDates--) | Λαμβάνει μια σημαία που καθορίζει εάν οι ημερομηνίες λήξης δραστηριοτήτων πρέπει να προγραμματιστούν ως οι αναμενόμενες ημερομηνίες λήξης. |
### getBaselineProjects() {#getBaselineProjects--}
```
public final Project[] getBaselineProjects()
```


Λαμβάνει τον πίνακα των βασικών έργων του τρέχοντος έργου. Ισχύει για έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενα βασικά στοιχεία.

**Returns:**
com.aspose.tasks.Project[] - πίνακας των βασικών έργων του τρέχοντος έργου.
### getCriticalActivitiesDefiningMethod() {#getCriticalActivitiesDefiningMethod--}
```
public final int getCriticalActivitiesDefiningMethod()
```


Λαμβάνει τη μέθοδο για τον ορισμό κρίσιμων δραστηριοτήτων: Longest Path ή Total Float.

**Returns:**
int - η μέθοδος για τον ορισμό κρίσιμων δραστηριοτήτων: Longest Path ή Total Float.
### getCriticalTotalFloatLimit() {#getCriticalTotalFloatLimit--}
```
public final Double getCriticalTotalFloatLimit()
```


Λαμβάνει την τιμή κατωφλίου που χρησιμοποιείται για τον ορισμό κρίσιμων δραστηριοτήτων εάν χρησιμοποιείται η μέθοδος TotalFloat.

**Returns:**
java.lang.Double - η τιμή κατωφλίου που χρησιμοποιείται για τον ορισμό κρίσιμων δραστηριοτήτων εάν χρησιμοποιείται η μέθοδος TotalFloat.
### getCurrentBaselineProjectId() {#getCurrentBaselineProjectId--}
```
public final int getCurrentBaselineProjectId()
```


Λαμβάνει το Id του τρέχοντος βασικού έργου. Ισχύει για έργα που διαβάζονται από αρχεία Primavera XML που περιέχουν εξαγόμενα βασικά στοιχεία.

**Returns:**
int - Id του τρέχοντος βασικού έργου.
### getIgnoreOtherProjectRelationships() {#getIgnoreOtherProjectRelationships--}
```
public final boolean getIgnoreOtherProjectRelationships()
```


Λαμβάνει μια σημαία που καθορίζει εάν θα αγνοηθούν οι σχέσεις δραστηριοτήτων μεταξύ έργων.

**Returns:**
boolean - μια σημαία που ορίζει αν θα αγνοηθούν οι σχέσεις δραστηριοτήτων μεταξύ έργων.
### getMakeOpenEndedActivitiesCritical() {#getMakeOpenEndedActivitiesCritical--}
```
public final boolean getMakeOpenEndedActivitiesCritical()
```


Λαμβάνει μια σημαία που καθορίζει εάν οι δραστηριότητες πρέπει να σημειωθούν ως κρίσιμες κατά τον προγραμματισμό του έργου.

**Returns:**
boolean - μια σημαία που ορίζει αν οι δραστηριότητες πρέπει να σημειώνονται ως κρίσιμες κατά τον προγραμματισμό του έργου.
### getRelationshipLagCalendar() {#getRelationshipLagCalendar--}
```
public final int getRelationshipLagCalendar()
```


Λαμβάνει μια επιλογή που καθορίζει ποιο ημερολόγιο θα χρησιμοποιηθεί για τον προγραμματισμό του καθυστέρησης σχέσης (Relationship Lag) σε έργα Primavera.

**Returns:**
int - μια επιλογή που ορίζει ποιο ημερολόγιο θα χρησιμοποιηθεί για τον προγραμματισμό του καθυστέρησης σχέσης σε έργα Primavera.
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Λαμβάνει το σύντομο όνομα του έργου (Αναγνωριστικό έργου).

**Returns:**
java.lang.String - σύντομο όνομα του έργου (Αναγνωριστικό έργου).
### getUseExpectedFinishDates() {#getUseExpectedFinishDates--}
```
public final boolean getUseExpectedFinishDates()
```


Λαμβάνει μια σημαία που καθορίζει εάν οι ημερομηνίες λήξης δραστηριοτήτων πρέπει να προγραμματιστούν ως οι αναμενόμενες ημερομηνίες λήξης.

**Returns:**
boolean - μια σημαία που ορίζει αν οι ημερομηνίες λήξης δραστηριοτήτων πρέπει να προγραμματιστούν ως οι αναμενόμενες ημερομηνίες λήξης.

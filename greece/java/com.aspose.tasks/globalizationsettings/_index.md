---
title: "GlobalizationSettings"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει τις ρυθμίσεις παγκοσμιοποίησης των έργων."
type: docs
weight: 114
url: /el/java/com.aspose.tasks/globalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public class GlobalizationSettings
```

Αναπαριστά τις ρυθμίσεις παγκοσμιοποίησης του έργου.

Ο συνιστώμενος τρόπος είναι να χρησιμοποιείτε culture-invariant literals ή formats σε όλο το έργο. Ωστόσο, εάν ένα έργο χρησιμοποιεί culture-specific literals, αυτή η κλάση μπορεί να χρησιμοποιηθεί για να βοηθήσει τη formula-calculation engine να αναλύσει αυτά τα literals.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GlobalizationSettings()](#GlobalizationSettings--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getFalseLiteral()](#getFalseLiteral--) | Επιστρέφει μια συμβολοσειρά για το boolean 'false' literal που χρησιμοποιείται σε τύπο. |
| [getFormulaDateNA()](#getFormulaDateNA--) | Επιστρέφει το literal "NA" (κενή τιμή) που χρησιμοποιείται σε τύπο για πεδίο ημερομηνίας. |
| [getTrueLiteral()](#getTrueLiteral--) | Επιστρέφει μια συμβολοσειρά για το boolean 'true' literal που χρησιμοποιείται σε τύπο. |
### GlobalizationSettings() {#GlobalizationSettings--}
```
public GlobalizationSettings()
```


### getFalseLiteral() {#getFalseLiteral--}
```
public String getFalseLiteral()
```


Επιστρέφει μια συμβολοσειρά για το boolean 'false' literal που χρησιμοποιείται σε τύπο.

**Returns:**
java.lang.String - μια συμβολοσειρά για το λογικό 'false' κυριολεκτικό που χρησιμοποιείται σε τύπο.
### getFormulaDateNA() {#getFormulaDateNA--}
```
public String getFormulaDateNA()
```


Επιστρέφει το literal "NA" (κενή τιμή) που χρησιμοποιείται σε τύπο για πεδίο ημερομηνίας.

**Returns:**
java.lang.String - \"NA\" (κενή τιμή) κυριολεκτικό που χρησιμοποιείται σε τύπο για πεδίο ημερομηνίας.
### getTrueLiteral() {#getTrueLiteral--}
```
public String getTrueLiteral()
```


Επιστρέφει μια συμβολοσειρά για το boolean 'true' literal που χρησιμοποιείται σε τύπο.

**Returns:**
java.lang.String - μια συμβολοσειρά για το λογικό 'true' κυριολεκτικό που χρησιμοποιείται σε τύπο.

---
title: "TimescaleFitBehavior"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αναπαριστά μια συμπεριφορά που χρησιμοποιείται για την ευθυγράμμιση της περιοχής κλίμακας χρόνου με το πλάτος της σελίδας."
type: docs
weight: 324
url: /el/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Αναπαριστά μια συμπεριφορά που χρησιμοποιείται για την ευθυγράμμιση της περιοχής κλίμακας χρόνου με το πλάτος της σελίδας.
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
| [DefinedInView](#DefinedInView) | Η ενότητα του ημερολογίου αποδίδεται σύμφωνα με την ιδιότητα View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage της αποδοθείσας προβολής. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Η ενότητα του ημερολογίου αποδίδεται ακριβώς μέχρι το EndDate, ακόμη και αν υπάρχει κενός χώρος σε μια σελίδα. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Η ενότητα του ημερολογίου αποδίδεται μέχρι το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Η μηχανή απόδοσης θα προσπαθήσει να ευθυγραμμίσει τις ημερομηνίες ώστε το EndDate να ευθυγραμμίζεται με το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Η ενότητα του ημερολογίου αποδίδεται σύμφωνα με την ιδιότητα View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage της αποδοθείσας προβολής.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Η ενότητα του ημερολογίου αποδίδεται ακριβώς μέχρι το EndDate, ακόμη και αν υπάρχει κενός χώρος σε μια σελίδα.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Η ενότητα του ημερολογίου αποδίδεται μέχρι το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. Συνεπώς η τελευταία αποδοθείσα ημερομηνία μπορεί να υπερβαίνει το EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Η μηχανή απόδοσης θα προσπαθήσει να ευθυγραμμίσει τις ημερομηνίες ώστε το EndDate να ευθυγραμμίζεται με το τέλος (δεξιά πλευρά) της τελευταίας σελίδας. Συμφωνεί με την ενεργοποιημένη επιλογή "Page Setup \\ View \\ Fit timescale to end of page" του MS Project.


---
title: "IPageSavingCallback"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν κάθε σελίδα σε έγγραφο πολλαπλών σελίδων αποθηκεύεται σε ξεχωριστό ρεύμα."
type: docs
weight: 382
url: /el/java/com.aspose.tasks/ipagesavingcallback/
---
```
public interface IPageSavingCallback
```

Αντιπροσωπεύει μια κλήση επιστροφής που καλείται όταν κάθε σελίδα σε έγγραφο πολλαπλών σελίδων αποθηκεύεται σε ξεχωριστό ρεύμα.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [onFinish()](#onFinish--) | Μέθοδος που θα κληθεί όταν γραφτούν όλες οι σελίδες. |
| [pageSaving(PageSavingArgs args)](#pageSaving-com.aspose.tasks.PageSavingArgs-) | Η μέθοδος που θα κληθεί όταν μια σελίδα αποθηκευτεί σε ροή. |
### onFinish() {#onFinish--}
```
public abstract void onFinish()
```


Μέθοδος που θα κληθεί όταν γραφτούν όλες οι σελίδες.

### pageSaving(PageSavingArgs args) {#pageSaving-com.aspose.tasks.PageSavingArgs-}
```
public abstract void pageSaving(PageSavingArgs args)
```


Η μέθοδος που θα κληθεί όταν μια σελίδα αποθηκευτεί σε ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| args | [PageSavingArgs](../../com.aspose.tasks/pagesavingargs) | Τα επιχειρήματα αποθήκευσης της σελίδας. |


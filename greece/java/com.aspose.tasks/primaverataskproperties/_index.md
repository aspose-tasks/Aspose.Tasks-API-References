---
title: "PrimaveraTaskProperties"
second_title: "Αναφορά API του Aspose.Tasks for Java"
description: "Αντιπροσωπεύει ιδιότητες ειδικές για Primavera για μια εργασία που διαβάζεται από αρχεία Primavera XER ή P6XML."
type: docs
weight: 209
url: /el/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Αναπαριστά ιδιότητες ειδικές για Primavera για μια εργασία που διαβάστηκε από αρχεία Primavera (XER ή P6XML).
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getActivityId()](#getActivityId--) | Λαμβάνει ένα πεδίο id δραστηριότητας - το μοναδικό αναγνωριστικό μιας εργασίας που χρησιμοποιείται από Primavera. |
| [getActivityType()](#getActivityType--) | Λαμβάνει την τιμή του πεδίου 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Λαμβάνει την τιμή του πραγματικού κόστους εξόδων. |
| [getActualLaborCost()](#getActualLaborCost--) | Λαμβάνει την τιμή του πραγματικού κόστους εργασίας. |
| [getActualLaborUnits()](#getActualLaborUnits--) | Λαμβάνει την τιμή των πραγματικών μονάδων εργασίας. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Λαμβάνει την τιμή του πραγματικού κόστους υλικού. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Λαμβάνει την τιμή των πραγματικών μη εργασιακών μονάδων. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Λαμβάνει την τιμή του πραγματικού μη εργασιακού κόστους. |
| [getActualTotalCost()](#getActualTotalCost--) | Λαμβάνει τη συνολική τιμή των πραγματικών εξόδων. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους δαπάνης. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους εργασίας. |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους υλικού. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) μη εργασιακού κόστους. |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Λαμβάνει τη συνολική τιμή των προϋπολογισμένων (ή προγραμματισμένων) εξόδων. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Λαμβάνει την τιμή του ποσοστού ολοκλήρωσης διάρκειας. |
| [getDurationType()](#getDurationType--) | Λαμβάνει την τιμή του πεδίου 'Duration Type' της δραστηριότητας. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Λαμβάνει την τιμή του πεδίου '% Complete Type' της δραστηριότητας. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Λαμβάνει την τιμή του Physical Percent Complete. |
| [getPlannedDuration()](#getPlannedDuration--) | Λαμβάνει την αρχική ή προγραμματισμένη διάρκεια — το συνολικό χρόνο εργασίας από την προγραμματισμένη ημερομηνία έναρξης της εργασίας έως την προγραμματισμένη ημερομηνία λήξης. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Λαμβάνει την ημερομηνία του κύριου περιορισμού. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Λαμβάνει έναν τύπο του κύριου περιορισμού. |
| [getRawActivityType()](#getRawActivityType--) | Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Activity Type' της δραστηριότητας. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου '% Complete Type' της δραστηριότητας. |
| [getRawDurationType()](#getRawDurationType--) | Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Duration Type' της δραστηριότητας. |
| [getRawStatus()](#getRawStatus--) | Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Status' της δραστηριότητας. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Λαμβάνει την ημερομηνία πρώιμου λήξης - την ημερομηνία κατά την οποία η εναπομείνασα εργασία για τη δραστηριότητα προγραμματίζεται να ολοκληρωθεί. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Λαμβάνει την ημερομηνία πρώιμης έναρξης - την ημερομηνία κατά την οποία η εναπομείνασα εργασία για τη δραστηριότητα προγραμματίζεται να ξεκινήσει. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Λαμβάνει την τιμή του εναπομείναντος κόστους δαπάνης. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Λαμβάνει την τιμή των υπολειπόμενων μονάδων εργασίας. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Λαμβάνει την υπολειπόμενη ημερομηνία λήξης καθυστέρησης. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Λαμβάνει την υπολειπόμενη ημερομηνία έναρξης καθυστέρησης. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Λαμβάνει την τιμή των υπολειπόμενων μη εργασιακών μονάδων. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Λαμβάνει την ημερομηνία του δευτερεύοντος περιορισμού. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Λαμβάνει έναν τύπο δευτερεύοντος περιορισμού. |
| [getSequenceNumber()](#getSequenceNumber--) | Λαμβάνει τον αριθμό ακολουθίας του στοιχείου WBS (συνοπτικές εργασίες). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Λαμβάνει την τιμή του ποσοστού ολοκλήρωσης μονάδων. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Λαμβάνει ένα πεδίο id δραστηριότητας - το μοναδικό αναγνωριστικό μιας εργασίας που χρησιμοποιείται από Primavera.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
java.lang.String - ένα πεδίο id δραστηριότητας - ένας μοναδικός αναγνωριστής εργασίας που χρησιμοποιείται από το Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Λαμβάνει την τιμή του πεδίου 'Activity Type'.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
int - η τιμή του πεδίου 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Λαμβάνει την τιμή του πραγματικού κόστους εξόδων.

**Returns:**
java.math.BigDecimal - η τιμή του πραγματικού κόστους εξόδων.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Λαμβάνει την τιμή του πραγματικού κόστους εργασίας.

**Returns:**
java.math.BigDecimal - η τιμή του πραγματικού κόστους εργασίας.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Λαμβάνει την τιμή των πραγματικών μονάδων εργασίας.

**Returns:**
double - η τιμή των πραγματικών μονάδων εργασίας.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Λαμβάνει την τιμή του πραγματικού κόστους υλικού.

**Returns:**
java.math.BigDecimal - η τιμή του πραγματικού κόστους υλικού.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Λαμβάνει την τιμή των πραγματικών μη εργασιακών μονάδων.

**Returns:**
double - η τιμή των πραγματικών μη εργασιακών μονάδων.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Λαμβάνει την τιμή του πραγματικού μη εργασιακού κόστους.

**Returns:**
java.math.BigDecimal - η τιμή του πραγματικού κόστους μη εργασίας.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Λαμβάνει τη συνολική τιμή των πραγματικών εξόδων.

**Returns:**
java.math.BigDecimal - η συνολική τιμή των πραγματικών εξόδων.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους δαπάνης.

**Returns:**
java.math.BigDecimal - η τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους εξόδων.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους εργασίας.

**Returns:**
java.math.BigDecimal - η τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους εργασίας.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους υλικού.

**Returns:**
java.math.BigDecimal - η τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους υλικού.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Λαμβάνει την τιμή του προϋπολογισμένου (ή προγραμματισμένου) μη εργασιακού κόστους.

**Returns:**
java.math.BigDecimal - η τιμή του προϋπολογισμένου (ή προγραμματισμένου) κόστους μη εργασίας.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Λαμβάνει τη συνολική τιμή των προϋπολογισμένων (ή προγραμματισμένων) εξόδων.

**Returns:**
java.math.BigDecimal - η συνολική τιμή των προϋπολογισμένων (ή προγραμματισμένων) εξόδων.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Λαμβάνει την τιμή του ποσοστού ολοκλήρωσης διάρκειας.

**Returns:**
double - η τιμή του ποσοστού ολοκλήρωσης διάρκειας.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Λαμβάνει την τιμή του πεδίου 'Duration Type' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
int - η τιμή του πεδίου 'Duration Type' της δραστηριότητας.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Λαμβάνει την τιμή του πεδίου '% Complete Type' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
int - η τιμή του πεδίου '% Complete Type' της δραστηριότητας.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Λαμβάνει την τιμή του Physical Percent Complete.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
double - η τιμή του Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Λαμβάνει την αρχική ή προγραμματισμένη διάρκεια — το συνολικό χρόνο εργασίας από την προγραμματισμένη ημερομηνία έναρξης της εργασίας έως την προγραμματισμένη ημερομηνία λήξης.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Λαμβάνει την ημερομηνία του κύριου περιορισμού.

**Returns:**
java.util.Date - η ημερομηνία του κύριου περιορισμού.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Λαμβάνει έναν τύπο του κύριου περιορισμού.

**Returns:**
int - ένας τύπος του κύριου περιορισμού.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Activity Type' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
java.lang.String - ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο πηγής) του πεδίου 'Activity Type' της δραστηριότητας.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου '% Complete Type' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
java.lang.String - ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο πηγής) του πεδίου '% Complete Type' της δραστηριότητας.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Duration Type' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
java.lang.String - ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο πηγής) του πεδίου 'Duration Type' της δραστηριότητας.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Λαμβάνει την ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο προέλευσης) του πεδίου 'Status' της δραστηριότητας.

--------------------

Ισχύει μόνο για δραστηριότητες (μη συνοπτικές εργασίες).

**Returns:**
java.lang.String - ακατέργαστη αναπαράσταση κειμένου (όπως στο αρχείο πηγής) του πεδίου 'Status' της δραστηριότητας.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Λαμβάνει την ημερομηνία πρώιμου λήξης - την ημερομηνία κατά την οποία η εναπομείνασα εργασία για τη δραστηριότητα προγραμματίζεται να ολοκληρωθεί.

**Returns:**
java.util.Date - η προαναγκαία ημερομηνία λήξης - η ημερομηνία κατά την οποία η υπόλοιπη εργασία για τη δραστηριότητα προγραμματίζεται να ολοκληρωθεί.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Λαμβάνει την ημερομηνία πρώιμης έναρξης - την ημερομηνία κατά την οποία η εναπομείνασα εργασία για τη δραστηριότητα προγραμματίζεται να ξεκινήσει.

**Returns:**
java.util.Date - η προαναγκαία ημερομηνία έναρξης - η ημερομηνία κατά την οποία η υπόλοιπη εργασία για τη δραστηριότητα προγραμματίζεται να ξεκινήσει.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Λαμβάνει την τιμή του εναπομείναντος κόστους δαπάνης.

**Returns:**
java.math.BigDecimal - η τιμή του υπολειπόμενου κόστους εξόδων.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Λαμβάνει την τιμή των υπολειπόμενων μονάδων εργασίας.

**Returns:**
double - η τιμή των υπολειπόμενων μονάδων εργασίας.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Λαμβάνει την υπολειπόμενη ημερομηνία λήξης καθυστέρησης.

**Returns:**
java.util.Date - η καθυστερημένη ημερομηνία λήξης.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Λαμβάνει την υπολειπόμενη ημερομηνία έναρξης καθυστέρησης.

**Returns:**
java.util.Date - η καθυστερημένη ημερομηνία έναρξης.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Λαμβάνει την τιμή των υπολειπόμενων μη εργασιακών μονάδων.

**Returns:**
double - η τιμή των υπολειπόμενων μη εργασιακών μονάδων.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Λαμβάνει την ημερομηνία του δευτερεύοντος περιορισμού.

**Returns:**
java.util.Date - η ημερομηνία του δευτερεύοντος περιορισμού.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Λαμβάνει έναν τύπο δευτερεύοντος περιορισμού.

**Returns:**
int - ένας τύπος του δευτερεύοντος περιορισμού.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Λαμβάνει τον αριθμό ακολουθίας του στοιχείου WBS (συνοπτικές εργασίες). Χρησιμοποιείται για την ταξινόμηση των συνοπτικών εργασιών στο Primavera.

--------------------

Εφαρμόσιμο σε στοιχεία WBS (συνοπτικές εργασίες).

**Returns:**
int - ο αριθμός ακολουθίας του στοιχείου WBS (συνοπτικές εργασίες).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Λαμβάνει την τιμή του ποσοστού ολοκλήρωσης μονάδων.

**Returns:**
double - η τιμή του ποσοστού ολοκλήρωσης μονάδων.

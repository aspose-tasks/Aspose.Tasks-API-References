---
title: PrimaveraTaskProperties
second_title: Aspose.Tasks for Java API Reference
description: Represents Primavera-specific properties for a task read from Primavera files XER of P6XML.
type: docs
weight: 208
url: /java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Represents Primavera-specific properties for a task read from Primavera files (XER of P6XML).
## Methods

| Method | Description |
| --- | --- |
| [getActivityId()](#getActivityId--) | Gets an activity id field - a task's unique identifier used by Primavera. |
| [getActivityType()](#getActivityType--) | Gets the value of 'Activity Type' field. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Gets the value of actual expense cost. |
| [getActualLaborCost()](#getActualLaborCost--) | Gets the value of actual labor cost . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Gets the value of actual labor units. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Gets the value of actual material cost. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Gets the value of actual non labor units. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Gets the value of actual non labor cost . |
| [getActualTotalCost()](#getActualTotalCost--) | Gets the total value of actual costs. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Gets the value of budgeted (or planned) expense cost. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Gets the value of budgeted (or planned) labor cost . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Gets the value of of budgeted (or planned) material cost. |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Gets the value of budgeted (or planned) non labor cost . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Gets the total value of budgeted (or planned) costs. |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Gets the value of duration percent complete. |
| [getDurationType()](#getDurationType--) | Gets the value of 'Duration Type' field of the activity. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Gets the value of '% Complete Type' field of the activity. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Gets the value of Physical Percent Complete. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Gets the date of primary constraint. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Gets a type of primary constraint. |
| [getRawActivityType()](#getRawActivityType--) | Gets raw text representation (as in source file) of 'Activity Type' field of the activity. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Gets raw text representation (as in source file) of '% Complete Type' field of the activity. |
| [getRawDurationType()](#getRawDurationType--) | Gets raw text representation (as in source file) of 'Duration Type' field of the activity. |
| [getRawStatus()](#getRawStatus--) | Gets raw text representation (as in source file) of 'Status' field of the activity. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Gets remaining early finish date - the date when the remaining work for the activity is scheduled to be finished. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Gets remaining early start date - the date when the remaining work for the activity is scheduled to begin. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Gets the value of remaining expense cost. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Gets the value of remaining labor units. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Gets remaining late finish date. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Gets remaining late start date. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Gets the value of remaining non labor units. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Gets the date of secondary constraint. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Gets a type of secondary constraint. |
| [getSequenceNumber()](#getSequenceNumber--) | Gets the sequence number of the WBS item (summary tasks). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Gets the value of units percent complete. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Gets an activity id field - a task's unique identifier used by Primavera.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - an activity id field - a task's unique identifier used by Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Gets the value of 'Activity Type' field.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
int - the value of 'Activity Type' field.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Gets the value of actual expense cost.

**Returns:**
java.math.BigDecimal - the value of actual expense cost.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Gets the value of actual labor cost .

**Returns:**
java.math.BigDecimal - the value of actual labor cost .
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Gets the value of actual labor units.

**Returns:**
double - the value of actual labor units.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Gets the value of actual material cost.

**Returns:**
java.math.BigDecimal - the value of actual material cost.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Gets the value of actual non labor units.

**Returns:**
double - the value of actual non labor units.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Gets the value of actual non labor cost .

**Returns:**
java.math.BigDecimal - the value of actual non labor cost .
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Gets the total value of actual costs.

**Returns:**
java.math.BigDecimal - the total value of actual costs.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Gets the value of budgeted (or planned) expense cost.

**Returns:**
java.math.BigDecimal - the value of budgeted (or planned) expense cost.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Gets the value of budgeted (or planned) labor cost .

**Returns:**
java.math.BigDecimal - the value of budgeted (or planned) labor cost .
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Gets the value of of budgeted (or planned) material cost.

**Returns:**
java.math.BigDecimal - the value of of budgeted (or planned) material cost.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Gets the value of budgeted (or planned) non labor cost .

**Returns:**
java.math.BigDecimal - the value of budgeted (or planned) non labor cost .
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Gets the total value of budgeted (or planned) costs.

**Returns:**
java.math.BigDecimal - the total value of budgeted (or planned) costs.
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Gets the value of duration percent complete.

**Returns:**
double - the value of duration percent complete.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Gets the value of 'Duration Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
int - the value of 'Duration Type' field of the activity.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Gets the value of '% Complete Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
int - the value of '% Complete Type' field of the activity.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Gets the value of Physical Percent Complete.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
double - the value of Physical Percent Complete.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Gets the date of primary constraint.

**Returns:**
java.util.Date - the date of primary constraint.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Gets a type of primary constraint.

**Returns:**
int - a type of primary constraint.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Gets raw text representation (as in source file) of 'Activity Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Activity Type' field of the activity.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Gets raw text representation (as in source file) of '% Complete Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of '% Complete Type' field of the activity.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Gets raw text representation (as in source file) of 'Duration Type' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Duration Type' field of the activity.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Gets raw text representation (as in source file) of 'Status' field of the activity.

--------------------

Applicable only to activities (non-summary tasks).

**Returns:**
java.lang.String - raw text representation (as in source file) of 'Status' field of the activity.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Gets remaining early finish date - the date when the remaining work for the activity is scheduled to be finished.

**Returns:**
java.util.Date - remaining early finish date - the date when the remaining work for the activity is scheduled to be finished.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Gets remaining early start date - the date when the remaining work for the activity is scheduled to begin.

**Returns:**
java.util.Date - remaining early start date - the date when the remaining work for the activity is scheduled to begin.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Gets the value of remaining expense cost.

**Returns:**
java.math.BigDecimal - the value of remaining expense cost.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Gets the value of remaining labor units.

**Returns:**
double - the value of remaining labor units.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Gets remaining late finish date.

**Returns:**
java.util.Date - remaining late finish date.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Gets remaining late start date.

**Returns:**
java.util.Date - remaining late start date.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Gets the value of remaining non labor units.

**Returns:**
double - the value of remaining non labor units.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Gets the date of secondary constraint.

**Returns:**
java.util.Date - the date of secondary constraint.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Gets a type of secondary constraint.

**Returns:**
int - a type of secondary constraint.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Gets the sequence number of the WBS item (summary tasks). It is used to sort summary tasks in Primavera.

--------------------

Applicable to WBS items (summary tasks).

**Returns:**
int - the sequence number of the WBS item (summary tasks).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Gets the value of units percent complete.

**Returns:**
double - the value of units percent complete.

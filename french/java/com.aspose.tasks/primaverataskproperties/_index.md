---
title: "PrimaveraTaskProperties"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les propriétés spécifiques à Primavera pour une tâche lue à partir des fichiers Primavera XER ou P6XML."
type: docs
weight: 209
url: /fr/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Représente les propriétés spécifiques à Primavera pour une tâche lue à partir de fichiers Primavera (XER ou P6XML).
## Méthodes

| Méthode | Description |
| --- | --- |
| [getActivityId()](#getActivityId--) | Obtient le champ d'identifiant d'activité – l'identifiant unique d'une tâche utilisé par Primavera. |
| [getActivityType()](#getActivityType--) | Obtient la valeur du champ 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Obtient la valeur du coût réel des dépenses. |
| [getActualLaborCost()](#getActualLaborCost--) | Obtient la valeur du coût réel de la main-d'œuvre . |
| [getActualLaborUnits()](#getActualLaborUnits--) | Obtient la valeur des unités réelles de main-d'œuvre. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Obtient la valeur du coût réel des matériaux. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Obtient la valeur des unités réelles non liées à la main-d'œuvre. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Obtient la valeur du coût réel non lié à la main-d'œuvre . |
| [getActualTotalCost()](#getActualTotalCost--) | Obtient la valeur totale des coûts réels. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Obtient la valeur du coût budgété (ou prévu) des dépenses. |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Obtient la valeur du coût budgété (ou prévu) de la main-d'œuvre . |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Obtient la valeur du coût budgété (ou prévu) des matériaux |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Obtient la valeur du coût budgété (ou prévu) non lié à la main-d'œuvre . |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Obtient la valeur totale des coûts budgétés (ou prévus). |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Obtient la valeur du pourcentage d'achèvement de la durée. |
| [getDurationType()](#getDurationType--) | Obtient la valeur du champ 'Duration Type' de l'activité. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Obtient la valeur du champ '% Complete Type' de l'activité. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Obtient la valeur du pourcentage d'achèvement physique. |
| [getPlannedDuration()](#getPlannedDuration--) | Obtient la durée originale ou prévue -- le temps de travail total entre la date de début prévue de la tâche et la date de fin prévue.. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Obtient la date de la contrainte principale. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Obtient le type de contrainte principale. |
| [getRawActivityType()](#getRawActivityType--) | Obtient la représentation texte brute (comme dans le fichier source) du champ 'Activity Type' de l'activité. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Obtient la représentation texte brute (comme dans le fichier source) du champ '% Complete Type' de l'activité. |
| [getRawDurationType()](#getRawDurationType--) | Obtient la représentation texte brute (comme dans le fichier source) du champ 'Duration Type' de l'activité. |
| [getRawStatus()](#getRawStatus--) | Obtient la représentation texte brute (comme dans le fichier source) du champ 'Status' de l'activité. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Obtient la date de fin anticipée restante - la date à laquelle le travail restant pour l'activité doit être terminé. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Obtient la date de début anticipée restante - la date à laquelle le travail restant pour l'activité doit commencer. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Obtient la valeur du coût restant des dépenses. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Obtient la valeur des unités de travail restantes. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Obtient la date de fin tardive restante. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Obtient la date de début tardif restante. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Obtient la valeur des unités non travaillées restantes. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Obtient la date de la contrainte secondaire. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Obtient un type de contrainte secondaire. |
| [getSequenceNumber()](#getSequenceNumber--) | Obtient le numéro de séquence de l'élément WBS (tâches de synthèse). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Obtient la valeur du pourcentage d'achèvement des unités. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Obtient le champ d'identifiant d'activité – l'identifiant unique d'une tâche utilisé par Primavera.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
java.lang.String - un champ d'identifiant d'activité - l'identifiant unique d'une tâche utilisé par Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Obtient la valeur du champ 'Activity Type'.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
int - la valeur du champ 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Obtient la valeur du coût réel des dépenses.

**Returns:**
java.math.BigDecimal - la valeur du coût réel des dépenses.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Obtient la valeur du coût réel de la main-d'œuvre .

**Returns:**
java.math.BigDecimal - la valeur du coût réel du travail.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Obtient la valeur des unités réelles de main-d'œuvre.

**Returns:**
double - la valeur des unités de travail réelles.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Obtient la valeur du coût réel des matériaux.

**Returns:**
java.math.BigDecimal - la valeur du coût réel des matériaux.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Obtient la valeur des unités réelles non liées à la main-d'œuvre.

**Returns:**
double - la valeur des unités non travaillées réelles.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Obtient la valeur du coût réel non lié à la main-d'œuvre .

**Returns:**
java.math.BigDecimal - la valeur du coût réel non lié au travail.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Obtient la valeur totale des coûts réels.

**Returns:**
java.math.BigDecimal - la valeur totale des coûts réels.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Obtient la valeur du coût budgété (ou prévu) des dépenses.

**Returns:**
java.math.BigDecimal - la valeur du coût budgété (ou prévu) des dépenses.
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Obtient la valeur du coût budgété (ou prévu) de la main-d'œuvre .

**Returns:**
java.math.BigDecimal - la valeur du coût budgété (ou prévu) du travail.
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Obtient la valeur du coût budgété (ou prévu) des matériaux

**Returns:**
java.math.BigDecimal - la valeur du coût budgété (ou prévu) des matériaux.
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Obtient la valeur du coût budgété (ou prévu) non lié à la main-d'œuvre .

**Returns:**
java.math.BigDecimal - la valeur du coût budgété (ou prévu) non lié au travail.
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Obtient la valeur totale des coûts budgétés (ou prévus).

**Returns:**
java.math.BigDecimal - la valeur totale des coûts budgétés (ou prévus).
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Obtient la valeur du pourcentage d'achèvement de la durée.

**Returns:**
double - la valeur du pourcentage d'achèvement de la durée.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Obtient la valeur du champ 'Duration Type' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
int - la valeur du champ 'Duration Type' de l'activité.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Obtient la valeur du champ '% Complete Type' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
int - la valeur du champ '% Complete Type' de l'activité.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Obtient la valeur du pourcentage d'achèvement physique.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
double - la valeur de Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Obtient la durée originale ou prévue -- le temps de travail total entre la date de début prévue de la tâche et la date de fin prévue..

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Obtient la date de la contrainte principale.

**Returns:**
java.util.Date - la date de la contrainte principale.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Obtient le type de contrainte principale.

**Returns:**
int - un type de contrainte principale.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Obtient la représentation texte brute (comme dans le fichier source) du champ 'Activity Type' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
java.lang.String - représentation texte brute (comme dans le fichier source) du champ 'Activity Type' de l'activité.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Obtient la représentation texte brute (comme dans le fichier source) du champ '% Complete Type' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
java.lang.String - représentation texte brute (comme dans le fichier source) du champ '% Complete Type' de l'activité.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Obtient la représentation texte brute (comme dans le fichier source) du champ 'Duration Type' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
java.lang.String - représentation texte brute (comme dans le fichier source) du champ 'Duration Type' de l'activité.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Obtient la représentation texte brute (comme dans le fichier source) du champ 'Status' de l'activité.

--------------------

Applicable uniquement aux activités (tâches non résumées).

**Returns:**
java.lang.String - représentation texte brute (comme dans le fichier source) du champ 'Status' de l'activité.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Obtient la date de fin anticipée restante - la date à laquelle le travail restant pour l'activité doit être terminé.

**Returns:**
java.util.Date - date de fin anticipée restante - la date à laquelle le travail restant pour l'activité doit être terminé.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Obtient la date de début anticipée restante - la date à laquelle le travail restant pour l'activité doit commencer.

**Returns:**
java.util.Date - date de début anticipée restante - la date à laquelle le travail restant pour l'activité doit commencer.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Obtient la valeur du coût restant des dépenses.

**Returns:**
java.math.BigDecimal - la valeur du coût restant des dépenses.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Obtient la valeur des unités de travail restantes.

**Returns:**
double - la valeur des unités de travail restantes.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Obtient la date de fin tardive restante.

**Returns:**
java.util.Date - date de fin tardive restante.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Obtient la date de début tardif restante.

**Returns:**
java.util.Date - date de début tardive restante.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Obtient la valeur des unités non travaillées restantes.

**Returns:**
double - la valeur des unités non liées au travail restantes.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Obtient la date de la contrainte secondaire.

**Returns:**
java.util.Date - la date de la contrainte secondaire.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Obtient un type de contrainte secondaire.

**Returns:**
int - un type de contrainte secondaire.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Obtient le numéro de séquence de l'élément WBS (tâches de synthèse). Il est utilisé pour trier les tâches de synthèse dans Primavera.

--------------------

Applicable aux éléments WBS (tâches de synthèse).

**Returns:**
int - le numéro de séquence de l'élément WBS (tâches de synthèse).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Obtient la valeur du pourcentage d'achèvement des unités.

**Returns:**
double - la valeur du pourcentage d'achèvement des unités.

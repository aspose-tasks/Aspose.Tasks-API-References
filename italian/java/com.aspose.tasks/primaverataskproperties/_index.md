---
title: "PrimaveraTaskProperties"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta le proprietà specifiche di Primavera per un'attività letta dai file Primavera XER o P6XML."
type: docs
weight: 209
url: /it/java/com.aspose.tasks/primaverataskproperties/
---

**Inheritance:**
java.lang.Object
```
public final class PrimaveraTaskProperties
```

Rappresenta le proprietà specifiche di Primavera per un'attività letta dai file Primavera (XER o P6XML).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getActivityId()](#getActivityId--) | Ottiene il campo ID attività - l'identificatore univoco di un'attività utilizzato da Primavera. |
| [getActivityType()](#getActivityType--) | Ottiene il valore del campo 'Activity Type'. |
| [getActualExpenseCost()](#getActualExpenseCost--) | Ottiene il valore del costo spesa reale. |
| [getActualLaborCost()](#getActualLaborCost--) | Ottiene il valore del costo del lavoro effettivo. |
| [getActualLaborUnits()](#getActualLaborUnits--) | Ottiene il valore delle unità di lavoro effettive. |
| [getActualMaterialCost()](#getActualMaterialCost--) | Ottiene il valore del costo del materiale effettivo. |
| [getActualNonLaborUnits()](#getActualNonLaborUnits--) | Ottiene il valore delle unità non di lavoro effettive. |
| [getActualNonlaborCost()](#getActualNonlaborCost--) | Ottiene il valore del costo non di lavoro effettivo. |
| [getActualTotalCost()](#getActualTotalCost--) | Ottiene il valore totale dei costi effettivi. |
| [getBudgetedExpenseCost()](#getBudgetedExpenseCost--) | Ottiene il valore del costo di spesa preventivato (o pianificato). |
| [getBudgetedLaborCost()](#getBudgetedLaborCost--) | Ottiene il valore del costo del lavoro preventivato (o pianificato). |
| [getBudgetedMaterialCost()](#getBudgetedMaterialCost--) | Ottiene il valore del costo del materiale preventivato (o pianificato). |
| [getBudgetedNonlaborCost()](#getBudgetedNonlaborCost--) | Ottiene il valore del costo non di lavoro preventivato (o pianificato). |
| [getBudgetedTotalCost()](#getBudgetedTotalCost--) | Ottiene il valore totale dei costi preventivati (o pianificati). |
| [getDurationPercentComplete()](#getDurationPercentComplete--) | Ottiene il valore della percentuale di completamento della durata. |
| [getDurationType()](#getDurationType--) | Ottiene il valore del campo 'Duration Type' dell'attività. |
| [getPercentCompleteType()](#getPercentCompleteType--) | Ottiene il valore del campo '% Complete Type' dell'attività. |
| [getPhysicalPercentComplete()](#getPhysicalPercentComplete--) | Ottiene il valore di Physical Percent Complete. |
| [getPlannedDuration()](#getPlannedDuration--) | Ottiene la durata originale o pianificata -- il tempo totale di lavoro dalla data di inizio pianificata dell'attività alla data di fine pianificata. |
| [getPrimaryConstraintDate()](#getPrimaryConstraintDate--) | Ottiene la data del vincolo primario. |
| [getPrimaryConstraintType()](#getPrimaryConstraintType--) | Ottiene il tipo di vincolo primario. |
| [getRawActivityType()](#getRawActivityType--) | Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Activity Type' dell'attività. |
| [getRawCompletePercentType()](#getRawCompletePercentType--) | Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo '% Complete Type' dell'attività. |
| [getRawDurationType()](#getRawDurationType--) | Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Duration Type' dell'attività. |
| [getRawStatus()](#getRawStatus--) | Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Status' dell'attività. |
| [getRemainingEarlyFinish()](#getRemainingEarlyFinish--) | Ottiene la data di fine anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per terminare. |
| [getRemainingEarlyStart()](#getRemainingEarlyStart--) | Ottiene la data di inizio anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per iniziare. |
| [getRemainingExpenseCost()](#getRemainingExpenseCost--) | Ottiene il valore del costo di spesa residuo. |
| [getRemainingLaborUnits()](#getRemainingLaborUnits--) | Ottiene il valore delle unità di lavoro rimanenti. |
| [getRemainingLateFinish()](#getRemainingLateFinish--) | Ottiene la data di fine ritardata rimanente. |
| [getRemainingLateStart()](#getRemainingLateStart--) | Ottiene la data di inizio ritardata rimanente. |
| [getRemainingNonLaborUnits()](#getRemainingNonLaborUnits--) | Ottiene il valore delle unità non lavorative rimanenti. |
| [getSecondaryConstraintDate()](#getSecondaryConstraintDate--) | Ottiene la data del vincolo secondario. |
| [getSecondaryConstraintType()](#getSecondaryConstraintType--) | Ottiene un tipo di vincolo secondario. |
| [getSequenceNumber()](#getSequenceNumber--) | Ottiene il numero di sequenza dell'elemento WBS (attività di riepilogo). |
| [getUnitsPercentComplete()](#getUnitsPercentComplete--) | Ottiene il valore della percentuale di completamento delle unità. |
### getActivityId() {#getActivityId--}
```
public final String getActivityId()
```


Ottiene il campo ID attività - l'identificatore univoco di un'attività utilizzato da Primavera.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
java.lang.String - un campo ID attività - l'identificatore unico di un'attività utilizzato da Primavera.
### getActivityType() {#getActivityType--}
```
public final int getActivityType()
```


Ottiene il valore del campo 'Activity Type'.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
int - il valore del campo 'Activity Type'.
### getActualExpenseCost() {#getActualExpenseCost--}
```
public final BigDecimal getActualExpenseCost()
```


Ottiene il valore del costo spesa reale.

**Returns:**
java.math.BigDecimal - il valore del costo spesa effettivo.
### getActualLaborCost() {#getActualLaborCost--}
```
public final BigDecimal getActualLaborCost()
```


Ottiene il valore del costo del lavoro effettivo.

**Returns:**
java.math.BigDecimal - il valore del costo lavoro effettivo.
### getActualLaborUnits() {#getActualLaborUnits--}
```
public final double getActualLaborUnits()
```


Ottiene il valore delle unità di lavoro effettive.

**Returns:**
double - il valore delle unità lavoro effettive.
### getActualMaterialCost() {#getActualMaterialCost--}
```
public final BigDecimal getActualMaterialCost()
```


Ottiene il valore del costo del materiale effettivo.

**Returns:**
java.math.BigDecimal - il valore del costo materiale effettivo.
### getActualNonLaborUnits() {#getActualNonLaborUnits--}
```
public final double getActualNonLaborUnits()
```


Ottiene il valore delle unità non di lavoro effettive.

**Returns:**
double - il valore delle unità non lavorative effettive.
### getActualNonlaborCost() {#getActualNonlaborCost--}
```
public final BigDecimal getActualNonlaborCost()
```


Ottiene il valore del costo non di lavoro effettivo.

**Returns:**
java.math.BigDecimal - il valore del costo non lavorativo effettivo.
### getActualTotalCost() {#getActualTotalCost--}
```
public final BigDecimal getActualTotalCost()
```


Ottiene il valore totale dei costi effettivi.

**Returns:**
java.math.BigDecimal - il valore totale dei costi effettivi.
### getBudgetedExpenseCost() {#getBudgetedExpenseCost--}
```
public final BigDecimal getBudgetedExpenseCost()
```


Ottiene il valore del costo di spesa preventivato (o pianificato).

**Returns:**
java.math.BigDecimal - il valore del costo spesa preventivato (o pianificato).
### getBudgetedLaborCost() {#getBudgetedLaborCost--}
```
public final BigDecimal getBudgetedLaborCost()
```


Ottiene il valore del costo del lavoro preventivato (o pianificato).

**Returns:**
java.math.BigDecimal - il valore del costo lavoro preventivato (o pianificato).
### getBudgetedMaterialCost() {#getBudgetedMaterialCost--}
```
public final BigDecimal getBudgetedMaterialCost()
```


Ottiene il valore del costo del materiale preventivato (o pianificato).

**Returns:**
java.math.BigDecimal - il valore del costo materiale preventivato (o pianificato).
### getBudgetedNonlaborCost() {#getBudgetedNonlaborCost--}
```
public final BigDecimal getBudgetedNonlaborCost()
```


Ottiene il valore del costo non di lavoro preventivato (o pianificato).

**Returns:**
java.math.BigDecimal - il valore del costo non lavorativo preventivato (o pianificato).
### getBudgetedTotalCost() {#getBudgetedTotalCost--}
```
public final BigDecimal getBudgetedTotalCost()
```


Ottiene il valore totale dei costi preventivati (o pianificati).

**Returns:**
java.math.BigDecimal - il valore totale dei costi preventivati (o pianificati).
### getDurationPercentComplete() {#getDurationPercentComplete--}
```
public final double getDurationPercentComplete()
```


Ottiene il valore della percentuale di completamento della durata.

**Returns:**
double - il valore della percentuale di completamento della durata.
### getDurationType() {#getDurationType--}
```
public final int getDurationType()
```


Ottiene il valore del campo 'Duration Type' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
int - il valore del campo 'Duration Type' dell'attività.
### getPercentCompleteType() {#getPercentCompleteType--}
```
public final int getPercentCompleteType()
```


Ottiene il valore del campo '% Complete Type' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
int - il valore del campo '% Complete Type' dell'attività.
### getPhysicalPercentComplete() {#getPhysicalPercentComplete--}
```
public final double getPhysicalPercentComplete()
```


Ottiene il valore di Physical Percent Complete.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
double - il valore di Physical Percent Complete.
### getPlannedDuration() {#getPlannedDuration--}
```
public final Duration getPlannedDuration()
```


Ottiene la durata originale o pianificata -- il tempo totale di lavoro dalla data di inizio pianificata dell'attività alla data di fine pianificata.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the original or planned duration -- the total working time from the task planned start date to the planned finish date.
### getPrimaryConstraintDate() {#getPrimaryConstraintDate--}
```
public final Date getPrimaryConstraintDate()
```


Ottiene la data del vincolo primario.

**Returns:**
java.util.Date - la data del vincolo primario.
### getPrimaryConstraintType() {#getPrimaryConstraintType--}
```
public final int getPrimaryConstraintType()
```


Ottiene il tipo di vincolo primario.

**Returns:**
int - un tipo di vincolo primario.
### getRawActivityType() {#getRawActivityType--}
```
public final String getRawActivityType()
```


Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Activity Type' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
java.lang.String - rappresentazione testuale grezza (come nel file sorgente) del campo 'Activity Type' dell'attività.
### getRawCompletePercentType() {#getRawCompletePercentType--}
```
public final String getRawCompletePercentType()
```


Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo '% Complete Type' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
java.lang.String - rappresentazione testuale grezza (come nel file sorgente) del campo '% Complete Type' dell'attività.
### getRawDurationType() {#getRawDurationType--}
```
public final String getRawDurationType()
```


Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Duration Type' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
java.lang.String - rappresentazione testuale grezza (come nel file sorgente) del campo 'Duration Type' dell'attività.
### getRawStatus() {#getRawStatus--}
```
public final String getRawStatus()
```


Ottiene la rappresentazione del testo grezzo (come nel file sorgente) del campo 'Status' dell'attività.

--------------------

Applicabile solo alle attività (attività non di riepilogo).

**Returns:**
java.lang.String - rappresentazione testuale grezza (come nel file sorgente) del campo 'Status' dell'attività.
### getRemainingEarlyFinish() {#getRemainingEarlyFinish--}
```
public final Date getRemainingEarlyFinish()
```


Ottiene la data di fine anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per terminare.

**Returns:**
java.util.Date - data di fine anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per essere completato.
### getRemainingEarlyStart() {#getRemainingEarlyStart--}
```
public final Date getRemainingEarlyStart()
```


Ottiene la data di inizio anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per iniziare.

**Returns:**
java.util.Date - data di inizio anticipata residua - la data in cui il lavoro residuo per l'attività è programmato per iniziare.
### getRemainingExpenseCost() {#getRemainingExpenseCost--}
```
public final BigDecimal getRemainingExpenseCost()
```


Ottiene il valore del costo di spesa residuo.

**Returns:**
java.math.BigDecimal - il valore del costo residuo delle spese.
### getRemainingLaborUnits() {#getRemainingLaborUnits--}
```
public final double getRemainingLaborUnits()
```


Ottiene il valore delle unità di lavoro rimanenti.

**Returns:**
double - il valore delle unità di lavoro residue.
### getRemainingLateFinish() {#getRemainingLateFinish--}
```
public final Date getRemainingLateFinish()
```


Ottiene la data di fine ritardata rimanente.

**Returns:**
java.util.Date - data di fine tardiva residua.
### getRemainingLateStart() {#getRemainingLateStart--}
```
public final Date getRemainingLateStart()
```


Ottiene la data di inizio ritardata rimanente.

**Returns:**
java.util.Date - data di inizio tardiva residua.
### getRemainingNonLaborUnits() {#getRemainingNonLaborUnits--}
```
public final double getRemainingNonLaborUnits()
```


Ottiene il valore delle unità non lavorative rimanenti.

**Returns:**
double - il valore delle unità non di lavoro residue.
### getSecondaryConstraintDate() {#getSecondaryConstraintDate--}
```
public final Date getSecondaryConstraintDate()
```


Ottiene la data del vincolo secondario.

**Returns:**
java.util.Date - la data del vincolo secondario.
### getSecondaryConstraintType() {#getSecondaryConstraintType--}
```
public final int getSecondaryConstraintType()
```


Ottiene un tipo di vincolo secondario.

**Returns:**
int - un tipo di vincolo secondario.
### getSequenceNumber() {#getSequenceNumber--}
```
public final int getSequenceNumber()
```


Restituisce il numero di sequenza dell'elemento WBS (attività di riepilogo). Viene utilizzato per ordinare le attività di riepilogo in Primavera.

--------------------

Applicabile agli elementi WBS (attività di riepilogo).

**Returns:**
int - il numero di sequenza dell'elemento WBS (attività di riepilogo).
### getUnitsPercentComplete() {#getUnitsPercentComplete--}
```
public final double getUnitsPercentComplete()
```


Ottiene il valore della percentuale di completamento delle unità.

**Returns:**
double - il valore della percentuale di completamento delle unità.

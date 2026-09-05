---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta un'assegnazione di risorsa in un progetto."
type: docs
weight: 249
url: /it/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Rappresenta un'assegnazione di risorsa in un progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [delete()](#delete--) | Elimina l'assegnazione della risorsa dalla collezione delle assegnazioni del progetto. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getACWP()](#getACWP--) | Ottiene un valore di ACWP. |
| [getActualCost()](#getActualCost--) | Ottiene un valore di ActualCost. |
| [getActualFinish()](#getActualFinish--) | Ottiene un valore di ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Ottiene un valore di ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Ottiene un valore di ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Ottiene un valore di ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Ottiene un valore di ActualStart. |
| [getActualWork()](#getActualWork--) | Ottiene un valore di ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Ottiene un valore di ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Ottiene un valore di AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Ottiene un valore di AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Ottiene un valore di BCWP. |
| [getBCWS()](#getBCWS--) | Ottiene un valore di BCWS. |
| [getBaselines()](#getBaselines--) | Ottiene l'oggetto AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | Ottiene un valore di BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Ottiene un valore di BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Ottiene un valore di BudgetWork. |
| [getCV()](#getCV--) | Ottiene un valore di CV. |
| [getConfirmed()](#getConfirmed--) | Ottiene un valore che indica se Confirmed è impostato o meno. |
| [getCost()](#getCost--) | Ottiene un valore di Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Ottiene un valore di CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Ottiene un valore di CostVariance. |
| [getCreated()](#getCreated--) | Ottiene un valore di Created. |
| [getDelay()](#getDelay--) | Ottiene un valore di Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Ottiene un'istanza della classe ExtendedAttributeCollection per questo oggetto. |
| [getFinish()](#getFinish--) | Ottiene un valore di Finish. |
| [getFinishVariance()](#getFinishVariance--) | Ottiene un valore di FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Ottiene un valore che indica se FixedMaterial è impostato o meno. |
| [getGuid()](#getGuid--) | Ottiene l'identificatore univoco per questa assegnazione. |
| [getHyperlink()](#getHyperlink--) | Ottiene un valore di Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Ottiene un valore di HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Ottiene un valore di HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Ottiene un valore di LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Ottiene un valore che indica se LinkedFields è impostato o meno. |
| [getMilestone()](#getMilestone--) | Ottiene un valore che indica se Milestone è impostato o meno. |
| [getNotesRTF()](#getNotesRTF--) | Ottiene le note di testo in formato RTF. |
| [getNotesText()](#getNotesText--) | Ottiene il testo semplice delle note estratto dai dati RTF. |
| [getOverallocated()](#getOverallocated--) | Ottiene un valore che indica se Overallocated è impostato o meno. |
| [getOvertimeCost()](#getOvertimeCost--) | Ottiene un valore di OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Ottiene un valore di OvertimeWork. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto genitore per questa assegnazione. |
| [getPeakUnits()](#getPeakUnits--) | Ottiene un valore di PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Ottiene un valore di PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Ottiene un valore di RateScale. |
| [getRegularWork()](#getRegularWork--) | Ottiene un valore di RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Ottiene un valore di RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Ottiene un valore di RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Ottiene un valore di RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Ottiene un valore di RemainingWork. |
| [getResource()](#getResource--) | La risorsa assegnata a un'attività. |
| [getResponsePending()](#getResponsePending--) | Ottiene un valore che indica se ResponsePending è impostato o meno. |
| [getResume()](#getResume--) | Ottiene un valore di Resume. |
| [getSV()](#getSV--) | Ottiene un valore di SV. |
| [getStart()](#getStart--) | Ottiene un valore di Start. |
| [getStartVariance()](#getStartVariance--) | Ottiene un valore di StartVariance. |
| [getStop()](#getStop--) | Ottiene un valore di Stop. |
| [getSummary()](#getSummary--) | Ottiene un valore che indica se Summary è impostato o meno. |
| [getTask()](#getTask--) | L'attività a cui è assegnata una risorsa. |
| [getTimephasedData()](#getTimephasedData--) | Ottiene l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente elementi di `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)). |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Restituisce l'oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) con le istanze di `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) all'interno delle date di inizio e fine fornite di [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Restituisce l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente istanze di `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) all'interno delle date di inizio e fine specificate del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Ottiene la quantità di lavoro timephased per l'intervallo di data e ora specificato. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Ottiene la quantità di lavoro timephased per l'intervallo di data e ora specificato. |
| [getUid()](#getUid--) | Ottiene un valore di Uid. |
| [getUnits()](#getUnits--) | Ottiene un valore di Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Ottiene un valore che indica se UpdateNeeded è impostato o meno. |
| [getVAC()](#getVAC--) | Ottiene un valore di VAC. |
| [getWork()](#getWork--) | Ottiene un valore di Work. |
| [getWorkContour()](#getWorkContour--) | Ottiene un valore di WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Ottiene un valore di WorkVariance. |
| [hasChildren()](#hasChildren--) | Ottiene un valore che indica che questa assegnazione di risorsa ha figli. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Ottiene un valore che indica se HasFixedRateUnits è impostato o meno. |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Genera un elenco di dati a fasi temporali. |
| [setACWP(double value)](#setACWP-double-) | Imposta un valore di ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Imposta un valore di ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Imposta un valore di ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Imposta un valore di ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Imposta un valore di ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Imposta un valore di ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Imposta un valore di ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Imposta un valore di ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Imposta un valore di AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Imposta un valore di AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Imposta un valore di BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Imposta un valore di BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Imposta un valore di BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Imposta un valore di BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Imposta un valore di BudgetWork. |
| [setCV(double value)](#setCV-double-) | Imposta un valore di CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Imposta un valore che indica se Confirmed è impostato o meno. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Imposta un valore di Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Imposta un valore di CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Imposta un valore di CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Imposta un valore di Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Imposta un valore di Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Imposta un'istanza della classe ExtendedAttributeCollection per questo oggetto. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Imposta un valore di Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Imposta un valore di FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Imposta un valore che indica se FixedMaterial è impostato o meno. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Imposta un valore che indica se HasFixedRateUnits è impostato o meno. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Imposta l'identificatore univoco per questa assegnazione. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Imposta un valore di Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Imposta un valore di HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Imposta un valore di HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Imposta un valore di LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Imposta un valore che indica se LinkedFields è impostato o meno. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Imposta le unità per l'assegnazione di una risorsa materiale con consumo variabile di materiale. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Imposta un valore che indica se Milestone è impostato o meno. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Imposta le note di testo in formato RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Imposta il testo semplice delle note estratto dai dati RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Imposta un valore che indica se Overallocated è impostato o meno. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Imposta un valore di OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Imposta un valore di PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Imposta un valore di PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Imposta un valore di RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Imposta un valore di RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Imposta un valore di RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Imposta un valore di RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Imposta un valore di RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | La risorsa assegnata a un'attività. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Imposta un valore che indica se ResponsePending è impostato o meno. |
| [setResume(Date value)](#setResume-java.util.Date-) | Imposta un valore di Resume. |
| [setSV(double value)](#setSV-double-) | Imposta un valore di SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Imposta un valore di Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Imposta un valore di StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Imposta un valore di Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Imposta un valore che indica se Summary è impostato o meno. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | L'attività a cui è assegnata una risorsa. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Imposta l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente gli elementi di `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe. |
| [setUid(int value)](#setUid-int-) | Imposta un valore di Uid. |
| [setUnits(double value)](#setUnits-double-) | Imposta un valore di Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Imposta un valore che indica se UpdateNeeded è impostato o meno. |
| [setVAC(double value)](#setVAC-double-) | Imposta un valore di VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Imposta un valore di Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Imposta un valore di WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Imposta un valore di WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Divide l'attività in due parti. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Genera un elenco di dati a fasi temporali basato sulla durata dell'attività e sulla data di inizio programmata. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa breve dell'istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Restituisce il valore a cui la proprietà è mappata in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Asn](../../com.aspose.tasks/asn) per ottenere la chiave della proprietà. |

**Returns:**
T - il valore a cui la proprietà è mappata in questo contenitore.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappa la proprietà specificata al valore specificato in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Asn](../../com.aspose.tasks/asn) per ottenere la chiave della proprietà. |
| val | T | il valore. |

### delete() {#delete--}
```
public final void delete()
```


Elimina l'assegnazione della risorsa dalla collezione delle assegnazioni del progetto.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | L'istanza specificata della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment) da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'istanza specificata della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment) ha lo stesso valore UID di questa istanza; altrimenti, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto da confrontare con questa istanza. |

**Returns:**
boolean - **True** se o è un ResourceAssignment che assegna la stessa risorsa e attività di questa istanza; altrimenti, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Ottiene un valore di ACWP.

**Returns:**
double - un valore di ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Ottiene un valore di ActualCost.

**Returns:**
java.math.BigDecimal - un valore di ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Ottiene un valore di ActualFinish.

**Returns:**
java.util.Date - un valore di ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Ottiene un valore di ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - un valore di ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Ottiene un valore di ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Ottiene un valore di ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Ottiene un valore di ActualStart.

**Returns:**
java.util.Date - un valore di ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Ottiene un valore di ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Ottiene un valore di ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Ottiene un valore di AssignmentOwner.

**Returns:**
java.lang.String - un valore di AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Ottiene un valore di AssignmentOwnerGuid.

**Returns:**
java.lang.String - un valore di AssignmentOwnerGuid.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Ottiene un valore di BCWP.

**Returns:**
double - un valore di BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Ottiene un valore di BCWS.

**Returns:**
double - un valore di BCWS.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


Ottiene l'oggetto AssignmentBaselineCollection. La raccolta di valori di baseline associati a un'assegnazione.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Ottiene un valore di BookingType.

**Returns:**
int - un valore di BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Ottiene un valore di BudgetCost.

**Returns:**
java.math.BigDecimal - un valore di BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Ottiene un valore di BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Ottiene un valore di CV.

**Returns:**
double - un valore di CV.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Ottiene un valore che indica se Confirmed è impostato o meno.

**Returns:**
boolean - un valore che indica se Confirmed è impostato o meno.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ottiene un valore di Cost.

**Returns:**
java.math.BigDecimal - un valore di Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Ottiene un valore di CostRateTableType.

**Returns:**
int - un valore di CostRateTableType.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Ottiene un valore di CostVariance.

**Returns:**
double - un valore di CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Ottiene un valore di Created.

**Returns:**
java.util.Date - un valore di Created.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Ottiene un valore di Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Ottiene un'istanza della classe ExtendedAttributeCollection per questo oggetto.

--------------------

Lettura supportata solo per il formato XML.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ottiene un valore di Finish.

**Returns:**
java.util.Date - un valore di Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Ottiene un valore di FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Ottiene un valore che indica se FixedMaterial è impostato o meno.

**Returns:**
boolean - un valore che indica se FixedMaterial è impostato o meno.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Ottiene l'identificatore univoco per questa assegnazione.

**Returns:**
java.util.UUID - identificatore univoco per questa assegnazione.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Ottiene un valore di Hyperlink.

**Returns:**
java.lang.String - un valore di Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Ottiene un valore di HyperlinkAddress.

**Returns:**
java.lang.String - un valore di HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Ottiene un valore di HyperlinkSubAddress.

**Returns:**
java.lang.String - un valore di HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Riservato per uso interno.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \\{@inheritDoc\\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Ottiene un valore di LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Ottiene un valore che indica se LinkedFields è impostato o meno.

**Returns:**
boolean - un valore che indica se LinkedFields è impostato o meno.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Ottiene un valore che indica se Milestone è impostato o meno.

**Returns:**
boolean - un valore che indica se Milestone è impostato o meno.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Ottiene le note di testo in formato RTF.

--------------------

Supportato solo per i formati MPP.

**Returns:**
java.lang.String - le note di testo in formato RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Ottiene il testo semplice delle note estratto dai dati RTF.

**Returns:**
java.lang.String - testo semplice delle note estratto dai dati RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Ottiene un valore che indica se Overallocated è impostato o meno.

**Returns:**
boolean - un valore che indica se Overallocated è impostato o meno.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Ottiene un valore di OvertimeCost.

**Returns:**
java.math.BigDecimal - un valore di OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Ottiene un valore di OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ottiene il progetto genitore per questa assegnazione.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Ottiene un valore di PeakUnits.

**Returns:**
double - un valore di PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Ottiene un valore di PercentWorkComplete.

**Returns:**
int - un valore di PercentWorkComplete.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Ottiene un valore di RateScale.

**Returns:**
int - un valore di RateScale.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Ottiene un valore di RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Ottiene un valore di RemainingCost.

**Returns:**
java.math.BigDecimal - un valore di RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Ottiene un valore di RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - un valore di RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Ottiene un valore di RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Ottiene un valore di RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


La risorsa assegnata a un'attività.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Ottiene un valore che indica se ResponsePending è impostato o meno.

**Returns:**
boolean - un valore che indica se ResponsePending è impostato o meno.
### getResume() {#getResume--}
```
public final Date getResume()
```


Ottiene un valore di Resume.

**Returns:**
java.util.Date - un valore di Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Ottiene un valore di SV.

**Returns:**
double - un valore di SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Ottiene un valore di Start.

**Returns:**
java.util.Date - un valore di Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Ottiene un valore di StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Ottiene un valore di Stop.

**Returns:**
java.util.Date - un valore di Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Ottiene un valore che indica se Summary è impostato o meno.

**Returns:**
boolean - un valore che indica se Summary è impostato o meno.
### getTask() {#getTask--}
```
public final Task getTask()
```


L'attività a cui è assegnata una risorsa.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Ottiene l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente elementi di `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)).

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Restituisce l'oggetto [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) con le istanze di `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) all'interno delle date di inizio e fine fornite di [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | La data di inizio per i dati a intervalli temporali. |
| fine | java.util.Date | La data di fine per i dati a intervalli temporali. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Restituisce l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente istanze di `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) all'interno delle date di inizio e fine specificate del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | La data di inizio per i dati a intervalli temporali. |
| fine | java.util.Date | La data di fine per i dati a intervalli temporali. |
| timephasedType | byte | Il tipo di dati a intervalli temporali ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Ottiene la quantità di lavoro timephased per l'intervallo di data e ora specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Inizio dell'intervallo di data e ora. |
| fine | java.util.Date | Fine dell'intervallo di data e ora. |

**Returns:**
double - quantità di lavoro timephased per l'intervallo di data e ora specificato.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Ottiene la quantità di lavoro timephased per l'intervallo di data e ora specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | Inizio dell'intervallo di data e ora. |
| fine | java.util.Date | Fine dell'intervallo di data e ora. |
| timephasedDataType | byte | Tipo dei dati timephased da utilizzare. |

**Returns:**
double - quantità di lavoro timephased per l'intervallo di data e ora specificato.
### getUid() {#getUid--}
```
public final int getUid()
```


Ottiene un valore di Uid.

**Returns:**
int - un valore di Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Ottiene un valore di Units.

**Returns:**
double - un valore di Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Ottiene un valore che indica se UpdateNeeded è impostato o meno.

**Returns:**
boolean - un valore che indica se UpdateNeeded è impostato o meno.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Ottiene un valore di VAC.

**Returns:**
double - un valore di VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ottiene un valore di Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Ottiene un valore di WorkContour.

**Returns:**
int - un valore di WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Ottiene un valore di WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Ottiene un valore che indica che questa assegnazione di risorsa ha figli.

**Returns:**
boolean - Sempre falso.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Ottiene un valore che indica se HasFixedRateUnits è impostato o meno.

**Returns:**
boolean - un valore che indica se HasFixedRateUnits è impostato o meno.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Genera un elenco di dati a fasi temporali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | La data di inizio specificata. |
| time | double | Il tempo di lavoro specificato. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Il calendario di lavoro specificato. |
| elenco | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | L'elenco dei dati a intervalli temporali. |
| isWorking | boolean | Il flag specificato che indica se i dati a intervalli temporali sono operativi o meno. |
| type | int | Il tipo di dati a intervalli temporali specificato. |

**Returns:**
java.util.Date - Una data massima dall'elenco o data di inizio se l'elenco è vuoto.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Imposta un valore di ACWP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Imposta un valore di ActualCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Imposta un valore di ActualFinish.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Imposta un valore di ActualOvertimeCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Imposta un valore di ActualOvertimeWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Imposta un valore di ActualOvertimeWorkProtected.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Imposta un valore di ActualStart.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Imposta un valore di ActualWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Imposta un valore di ActualWorkProtected.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Imposta un valore di AssignmentOwner.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Imposta un valore di AssignmentOwnerGuid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di AssignmentOwnerGuid. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Imposta un valore di BCWP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Imposta un valore di BCWS.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Imposta un valore di BookingType.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di BookingType. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Imposta un valore di BudgetCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Imposta un valore di BudgetWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Imposta un valore di CV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di CV. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Imposta un valore che indica se Confirmed è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Confirmed è impostato o meno. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Imposta un valore di Cost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Imposta un valore di CostRateTableType.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di CostRateTableType. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Imposta un valore di CostVariance.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Imposta un valore di Created.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Created. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Imposta un valore di Delay.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Imposta un'istanza della classe ExtendedAttributeCollection per questo oggetto.

--------------------

Lettura supportata solo per il formato XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | un'istanza della classe ExtendedAttributeCollection per questo oggetto. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Imposta un valore di Finish.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Imposta un valore di FinishVariance.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Imposta un valore che indica se FixedMaterial è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se FixedMaterial è impostato o meno. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Imposta un valore che indica se HasFixedRateUnits è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se HasFixedRateUnits è impostato o meno. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Imposta l'identificatore univoco per questa assegnazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID | identificatore univoco per questa assegnazione. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Imposta un valore di Hyperlink.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Imposta un valore di HyperlinkAddress.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Imposta un valore di HyperlinkSubAddress.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Imposta un valore di LevelingDelay.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Imposta un valore che indica se LinkedFields è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se LinkedFields è impostato o meno. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Imposta le unità per l'assegnazione di una risorsa materiale con consumo variabile di materiale. Il consumo variabile di materiale significa che, man mano che la durata dell'assegnazione cambia, la quantità di materiali utilizzati varia proporzionalmente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| unità | double | Numero di unità accumulate nel periodo di tempo. |
|  | rateScaleType | int | Periodo di tempo in cui il valore dell'unità è accumulato. |

--------------------

Ad esempio, per impostare '123/mese', SetUnitsScaled(123D, RateScaleType.Month) dovrebbe essere chiamato. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Imposta un valore che indica se Milestone è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Milestone è impostato o meno. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Imposta le note di testo in formato RTF.

--------------------

Supportato solo per i formati MPP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | le note di testo in formato RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Imposta il testo semplice delle note estratto dai dati RTF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | testo semplice delle note estratto dai dati RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Imposta un valore che indica se Overallocated è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Overallocated è impostato o meno. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Imposta un valore di OvertimeCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Imposta un valore di OvertimeWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Imposta un valore di PeakUnits.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Imposta un valore di PercentWorkComplete.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di PercentWorkComplete. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Imposta un valore di RateScale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di RateScale. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Imposta un valore di RegularWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Imposta un valore di RemainingCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Imposta un valore di RemainingOvertimeCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Imposta un valore di RemainingOvertimeWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Imposta un valore di RemainingWork.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di RemainingWork. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


La risorsa assegnata a un'attività.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | la risorsa assegnata a un'attività. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Imposta un valore che indica se ResponsePending è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se ResponsePending è impostato o meno. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Imposta un valore di Resume.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Imposta un valore di SV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Imposta un valore di Start.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Imposta un valore di StartVariance.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Imposta un valore di Stop.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Imposta un valore che indica se Summary è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se Summary è impostato o meno. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


L'attività a cui è assegnata una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | l'attività a cui è assegnata una risorsa. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Imposta l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente gli elementi di `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | l'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenente elementi di `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Imposta un valore di Uid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Imposta un valore di Units.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Imposta un valore che indica se UpdateNeeded è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se UpdateNeeded è impostato o meno. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Imposta un valore di VAC.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Imposta un valore di Work.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Imposta un valore di WorkContour.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Imposta un valore di WorkVariance.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Divide l'attività in due parti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | L'inizio dell'interruzione del lavoro su cui basare la divisione. |
| fine | java.util.Date | La fine dell'interruzione del lavoro su cui basare la divisione. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Il calendario su cui basare la divisione. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Genera un elenco di dati a fasi temporali basato sulla durata dell'attività e sulla data di inizio programmata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Il calendario da cui generare i dati a intervalli temporali. |

### toString() {#toString--}
```
public String toString()
```


Restituisce una rappresentazione stringa breve dell'istanza della classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche.

**Returns:**
java.lang.String - stringa breve che rappresenta l'oggetto di assegnazione.

---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een resource-toewijzing in een project voor."
type: docs
weight: 249
url: /nl/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Stelt een resource-toewijzing in een project voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [delete()](#delete--) | Verwijdert resource assignment uit de collectie van projecttoewijzingen. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [ResourceAssignment](../../com.aspose.tasks/resourceassignment) klasse. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getACWP()](#getACWP--) | Haalt een waarde van ACWP op. |
| [getActualCost()](#getActualCost--) | Haalt een waarde van ActualCost op. |
| [getActualFinish()](#getActualFinish--) | Haalt een waarde van ActualFinish op. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Haalt een waarde van ActualOvertimeCost op. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Haalt een waarde van ActualOvertimeWork op. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Haalt een waarde van ActualOvertimeWorkProtected op. |
| [getActualStart()](#getActualStart--) | Haalt een waarde van ActualStart op. |
| [getActualWork()](#getActualWork--) | Haalt een waarde van ActualWork op. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Haalt een waarde van ActualWorkProtected op. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Haalt een waarde van AssignmentOwner op. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Haalt een waarde van AssignmentOwnerGuid op. |
| [getBCWP()](#getBCWP--) | Haalt een waarde van BCWP op. |
| [getBCWS()](#getBCWS--) | Haalt een waarde van BCWS op. |
| [getBaselines()](#getBaselines--) | Haalt AssignmentBaselineCollection object op. |
| [getBookingType()](#getBookingType--) | Haalt een waarde van BookingType op. |
| [getBudgetCost()](#getBudgetCost--) | Haalt een waarde van BudgetCost op. |
| [getBudgetWork()](#getBudgetWork--) | Haalt een waarde van BudgetWork op. |
| [getCV()](#getCV--) | Haalt een waarde van CV op. |
| [getConfirmed()](#getConfirmed--) | Haalt een waarde op die aangeeft of Confirmed is ingesteld of niet. |
| [getCost()](#getCost--) | Haalt een waarde van Cost op. |
| [getCostRateTableType()](#getCostRateTableType--) | Haalt een waarde van CostRateTableType op. |
| [getCostVariance()](#getCostVariance--) | Haalt een waarde van CostVariance op. |
| [getCreated()](#getCreated--) | Haalt een waarde van Created op. |
| [getDelay()](#getDelay--) | Haalt een waarde van Delay op. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Haalt een instantie van de ExtendedAttributeCollection klasse voor dit object op. |
| [getFinish()](#getFinish--) | Haalt een waarde van Finish op. |
| [getFinishVariance()](#getFinishVariance--) | Haalt een waarde van FinishVariance op. |
| [getFixedMaterial()](#getFixedMaterial--) | Haalt een waarde op die aangeeft of FixedMaterial is ingesteld of niet. |
| [getGuid()](#getGuid--) | Haalt een unieke identifier op voor deze toewijzing. |
| [getHyperlink()](#getHyperlink--) | Haalt een waarde op van Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Haalt een waarde op van HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Haalt een waarde op van HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Haalt een waarde op van LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Haalt een waarde op die aangeeft of LinkedFields is ingesteld of niet. |
| [getMilestone()](#getMilestone--) | Haalt een waarde op die aangeeft of Milestone is ingesteld of niet. |
| [getNotesRTF()](#getNotesRTF--) | Haalt de tekstnotities op in RTF-indeling. |
| [getNotesText()](#getNotesText--) | Haalt de platte tekst van notities op die uit RTF-gegevens is geëxtraheerd. |
| [getOverallocated()](#getOverallocated--) | Haalt een waarde op die aangeeft of Overallocated is ingesteld of niet. |
| [getOvertimeCost()](#getOvertimeCost--) | Haalt een waarde op van OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Haalt een waarde op van OvertimeWork. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op voor deze toewijzing. |
| [getPeakUnits()](#getPeakUnits--) | Haalt een waarde op van PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Haalt een waarde op van PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Haalt een waarde op van RateScale. |
| [getRegularWork()](#getRegularWork--) | Haalt een waarde op van RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Haalt een waarde op van RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Haalt een waarde op van RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Haalt een waarde op van RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Haalt een waarde op van RemainingWork. |
| [getResource()](#getResource--) | De resource die aan een taak is toegewezen. |
| [getResponsePending()](#getResponsePending--) | Haalt een waarde op die aangeeft of ResponsePending is ingesteld of niet. |
| [getResume()](#getResume--) | Haalt een waarde op van Resume. |
| [getSV()](#getSV--) | Haalt een waarde op van SV. |
| [getStart()](#getStart--) | Haalt een waarde op van Start. |
| [getStartVariance()](#getStartVariance--) | Haalt een waarde op van StartVariance. |
| [getStop()](#getStop--) | Haalt een waarde op van Stop. |
| [getSummary()](#getSummary--) | Haalt een waarde op die aangeeft of Summary is ingesteld of niet. |
| [getTask()](#getTask--) | De taak waaraan een resource is toegewezen. |
| [getTimephasedData()](#getTimephasedData--) | Haalt de instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse op die elementen bevat van `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klasse. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Retourneert een [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object met de instanties van `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klasse binnen de opgegeven start- en einddatums van [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Retourneert de instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse die instanties bevat van `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klasse binnen de opgegeven start- en einddatums van de gespecificeerde [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval. |
| [getUid()](#getUid--) | Haalt een waarde op van Uid. |
| [getUnits()](#getUnits--) | Haalt een waarde op van Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Haalt een waarde op die aangeeft of UpdateNeeded is ingesteld of niet. |
| [getVAC()](#getVAC--) | Haalt een waarde op van VAC. |
| [getWork()](#getWork--) | Haalt een waarde op van Work. |
| [getWorkContour()](#getWorkContour--) | Haalt een waarde op van WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Haalt een waarde op van WorkVariance. |
| [hasChildren()](#hasChildren--) | Haalt een waarde op die aangeeft dat deze resource‑toewijzing onderliggende items heeft. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Haalt een waarde op die aangeeft of HasFixedRateUnits is ingesteld of niet. |
| [hashCode()](#hashCode--) | Retourneert een hashcode‑waarde voor de instantie van de [ResourceAssignment](../../com.aspose.tasks/resourceassignment)‑klasse. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Genereert een lijst met tijdsgephaseerde gegevens. |
| [setACWP(double value)](#setACWP-double-) | Stelt een waarde in voor ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Stelt een waarde in voor ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Stelt een waarde in voor ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Stelt een waarde in voor ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Stelt een waarde in voor AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Stelt een waarde in voor AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Stelt een waarde in voor BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Stelt een waarde in voor BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Stelt een waarde in voor BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Stelt een waarde in voor BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor BudgetWork. |
| [setCV(double value)](#setCV-double-) | Stelt een waarde in voor CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Stelt een waarde in die aangeeft of Confirmed is ingesteld of niet. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Stelt een waarde in voor Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Stelt een waarde in voor CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Stelt een waarde in voor CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Stelt een waarde in voor Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Stelt een waarde in voor Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Stelt een instantie van de ExtendedAttributeCollection‑klasse in voor dit object. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Stelt een waarde in voor Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Stelt een waarde in voor FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Stelt een waarde in die aangeeft of FixedMaterial is ingesteld of niet. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Stelt een waarde in die aangeeft of HasFixedRateUnits is ingesteld of niet. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Stelt een unieke identifier in voor deze toewijzing. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Stelt een waarde in voor Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Stelt een waarde in voor HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Stelt een waarde in voor HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Stelt een waarde in voor LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Stelt een waarde in die aangeeft of LinkedFields is ingesteld of niet. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Stelt eenheden in voor de toewijzing van een materiële resource met variabele materiaalconsumptie. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Stelt een waarde in die aangeeft of Milestone is ingesteld of niet. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Stelt de tekstnotities in RTF‑formaat in. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Stelt de platte tekst van notities in die uit RTF‑gegevens is gehaald. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Stelt een waarde in die aangeeft of Overallocated is ingesteld of niet. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Stelt een waarde in voor PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Stelt een waarde in voor PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Stelt een waarde in voor RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Stelt een waarde in voor RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | De resource die aan een taak is toegewezen. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Stelt een waarde in die aangeeft of ResponsePending is ingesteld of niet. |
| [setResume(Date value)](#setResume-java.util.Date-) | Stelt een waarde in voor Resume. |
| [setSV(double value)](#setSV-double-) | Stelt een waarde in voor SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Stelt een waarde in voor Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Stelt een waarde in voor StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Stelt een waarde in voor Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Stelt een waarde in die aangeeft of Summary is ingesteld of niet. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | De taak waaraan een resource is toegewezen. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Stelt de instantie van de klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in die elementen van `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) bevat. |
| [setUid(int value)](#setUid-int-) | Stelt een waarde van Uid in. |
| [setUnits(double value)](#setUnits-double-) | Stelt een waarde in voor Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Stelt een waarde in die aangeeft of UpdateNeeded is ingesteld of niet. |
| [setVAC(double value)](#setVAC-double-) | Stelt een waarde in voor VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Stelt een waarde van Work in. |
| [setWorkContour(int value)](#setWorkContour-int-) | Stelt een waarde in voor WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Stelt een waarde van WorkVariance in. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Splitst taak in twee delen. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Genereert een lijst met tijdgephaseerde gegevens op basis van de taakduur en de geplande startdatum. |
| [toString()](#toString--) | Retourneert een korte tekenreeksrepresentatie van de instantie van de klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Retourneert de waarde waaraan de eigenschap in deze container is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Asn](../../com.aspose.tasks/asn) voor het ophalen van de eigenschapssleutel. |

**Returns:**
T - de waarde waaraan de eigenschap in deze container is toegewezen.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Asn](../../com.aspose.tasks/asn) voor het ophalen van de eigenschapssleutel. |
| val | T | de waarde. |

### delete() {#delete--}
```
public final void delete()
```


Verwijdert resource assignment uit de collectie van projecttoewijzingen.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [ResourceAssignment](../../com.aspose.tasks/resourceassignment) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | De opgegeven instantie van de klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment) om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als de opgegeven instantie van de klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment) dezelfde UID-waarde heeft als deze instantie; anders, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| obj | java.lang.Object | Het object om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als o een ResourceAssignment is die dezelfde resource en taak toewijst als deze instantie; anders, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Haalt een waarde van ACWP op.

**Returns:**
double - een waarde van ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Haalt een waarde van ActualCost op.

**Returns:**
java.math.BigDecimal - een waarde van ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Haalt een waarde van ActualFinish op.

**Returns:**
java.util.Date - een waarde van ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Haalt een waarde van ActualOvertimeCost op.

**Returns:**
java.math.BigDecimal - een waarde van ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Haalt een waarde van ActualOvertimeWork op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Haalt een waarde van ActualOvertimeWorkProtected op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Haalt een waarde van ActualStart op.

**Returns:**
java.util.Date - een waarde van ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Haalt een waarde van ActualWork op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Haalt een waarde van ActualWorkProtected op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Haalt een waarde van AssignmentOwner op.

**Returns:**
java.lang.String - een waarde van AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Haalt een waarde van AssignmentOwnerGuid op.

**Returns:**
java.lang.String - een waarde van AssignmentOwnerGuid.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Haalt een waarde van BCWP op.

**Returns:**
double - een waarde van BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Haalt een waarde van BCWS op.

**Returns:**
double - een waarde van BCWS.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


Haalt AssignmentBaselineCollection-object op. De collectie van baseline-waarden die aan een toewijzing zijn gekoppeld.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Haalt een waarde van BookingType op.

**Returns:**
int - een waarde van BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Haalt een waarde van BudgetCost op.

**Returns:**
java.math.BigDecimal - een waarde van BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Haalt een waarde van BudgetWork op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Haalt een waarde van CV op.

**Returns:**
double - een waarde van CV.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Haalt een waarde op die aangeeft of Confirmed is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of Confirmed is ingesteld of niet.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Haalt een waarde van Cost op.

**Returns:**
java.math.BigDecimal - een waarde van Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Haalt een waarde van CostRateTableType op.

**Returns:**
int - een waarde van CostRateTableType.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Haalt een waarde van CostVariance op.

**Returns:**
double - een waarde van CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Haalt een waarde van Created op.

**Returns:**
java.util.Date - een waarde van Created.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Haalt een waarde van Delay op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Haalt een instantie van de ExtendedAttributeCollection klasse voor dit object op.

--------------------

Alleen lezen ondersteund voor XML-indeling.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Haalt een waarde van Finish op.

**Returns:**
java.util.Date - een waarde van Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Haalt een waarde van FinishVariance op.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Haalt een waarde op die aangeeft of FixedMaterial is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of FixedMaterial is ingesteld of niet.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Haalt een unieke identifier op voor deze toewijzing.

**Returns:**
java.util.UUID - unieke identifier voor deze toewijzing.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Haalt een waarde op van Hyperlink.

**Returns:**
java.lang.String - een waarde van Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Haalt een waarde op van HyperlinkAddress.

**Returns:**
java.lang.String - een waarde van HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Haalt een waarde op van HyperlinkSubAddress.

**Returns:**
java.lang.String - een waarde van HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Gereserveerd voor intern gebruik.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Haalt een waarde op van LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Haalt een waarde op die aangeeft of LinkedFields is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of LinkedFields is ingesteld of niet.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Haalt een waarde op die aangeeft of Milestone is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of Milestone is ingesteld of niet.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Haalt de tekstnotities op in RTF-indeling.

--------------------

Alleen ondersteund voor MPP-formaten.

**Returns:**
java.lang.String - de tekstnotities in RTF-indeling.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Haalt de platte tekst van notities op die uit RTF-gegevens is geëxtraheerd.

**Returns:**
java.lang.String - platte tekst van notities geëxtraheerd uit RTF-gegevens.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Haalt een waarde op die aangeeft of Overallocated is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of Overallocated is ingesteld of niet.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Haalt een waarde op van OvertimeCost.

**Returns:**
java.math.BigDecimal - een waarde van OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Haalt een waarde op van OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt het bovenliggende project op voor deze toewijzing.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Haalt een waarde op van PeakUnits.

**Returns:**
double - een waarde van PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Haalt een waarde op van PercentWorkComplete.

**Returns:**
int - een waarde van PercentWorkComplete.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Haalt een waarde op van RateScale.

**Returns:**
int - een waarde van RateScale.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Haalt een waarde op van RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Haalt een waarde op van RemainingCost.

**Returns:**
java.math.BigDecimal - een waarde van RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Haalt een waarde op van RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - een waarde van RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Haalt een waarde op van RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Haalt een waarde op van RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


De resource die aan een taak is toegewezen.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Haalt een waarde op die aangeeft of ResponsePending is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of ResponsePending is ingesteld of niet.
### getResume() {#getResume--}
```
public final Date getResume()
```


Haalt een waarde op van Resume.

**Returns:**
java.util.Date - een waarde van Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Haalt een waarde op van SV.

**Returns:**
double - een waarde van SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Haalt een waarde op van Start.

**Returns:**
java.util.Date - een waarde van Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Haalt een waarde op van StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Haalt een waarde op van Stop.

**Returns:**
java.util.Date - een waarde van Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Haalt een waarde op die aangeeft of Summary is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of Summary is ingesteld of niet.
### getTask() {#getTask--}
```
public final Task getTask()
```


De taak waaraan een resource is toegewezen.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Haalt de instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse op die elementen bevat van `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klasse.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Retourneert een [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) object met de instanties van `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klasse binnen de opgegeven start- en einddatums van [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | De startdatum voor de tijdgephaseerde gegevens. |
| einde | java.util.Date | De einddatum voor de tijdgephaseerde gegevens. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Retourneert de instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse die instanties bevat van `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klasse binnen de opgegeven start- en einddatums van de gespecificeerde [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | De startdatum voor de tijdgephaseerde gegevens. |
| einde | java.util.Date | De einddatum voor de tijdgephaseerde gegevens. |
| timephasedType | byte | Het type tijdgephaseerde gegevens ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Begin van het datum‑tijdinterval. |
| einde | java.util.Date | Einde van het datum‑tijdinterval. |

**Returns:**
double - hoeveelheid tijdgephaseerd werk voor het opgegeven datum‑tijdinterval.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Haalt de hoeveelheid tijdgephaseerd werk op voor het opgegeven datum‑tijdinterval.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Begin van het datum‑tijdinterval. |
| einde | java.util.Date | Einde van het datum‑tijdinterval. |
| timephasedDataType | byte | Type van de te gebruiken tijdgephaseerde gegevens. |

**Returns:**
double - hoeveelheid tijdgephaseerd werk voor het opgegeven datum‑tijdinterval.
### getUid() {#getUid--}
```
public final int getUid()
```


Haalt een waarde op van Uid.

**Returns:**
int - een waarde van Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Haalt een waarde op van Units.

**Returns:**
double - een waarde van Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Haalt een waarde op die aangeeft of UpdateNeeded is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of UpdateNeeded is ingesteld of niet.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Haalt een waarde op van VAC.

**Returns:**
double - een waarde van VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Haalt een waarde op van Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Haalt een waarde op van WorkContour.

**Returns:**
int - een waarde van WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Haalt een waarde op van WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Haalt een waarde op die aangeeft dat deze resource‑toewijzing onderliggende items heeft.

**Returns:**
boolean - Altijd onwaar.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Haalt een waarde op die aangeeft of HasFixedRateUnits is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of HasFixedRateUnits is ingesteld of niet.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode‑waarde voor de instantie van de [ResourceAssignment](../../com.aspose.tasks/resourceassignment)‑klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Genereert een lijst met tijdsgephaseerde gegevens.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | De opgegeven startdatum. |
| time | double | De opgegeven werktijd. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | De opgegeven werkkalender. |
| lijst | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | De lijst met tijdgephaseerde gegevens. |
| isWorking | boolean | De opgegeven vlag die aangeeft of tijdgephaseerde gegevens werken of niet. |
| type | int | Het opgegeven tijdgephaseerde gegevenstype. |

**Returns:**
java.util.Date - Een maximale datum uit de lijst of startdatum als de lijst leeg is.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Stelt een waarde in voor ACWP.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Stelt een waarde in voor ActualCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Stelt een waarde in voor ActualFinish.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Stelt een waarde in voor ActualOvertimeCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Stelt een waarde in voor ActualOvertimeWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Stelt een waarde in voor ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Stelt een waarde in voor ActualStart.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Stelt een waarde in voor ActualWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Stelt een waarde in voor ActualWorkProtected.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Stelt een waarde in voor AssignmentOwner.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Stelt een waarde in voor AssignmentOwnerGuid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van AssignmentOwnerGuid. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Stelt een waarde in voor BCWP.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Stelt een waarde in voor BCWS.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Stelt een waarde in voor BookingType.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van BookingType. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Stelt een waarde in voor BudgetCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Stelt een waarde in voor BudgetWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Stelt een waarde in voor CV.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van CV. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Stelt een waarde in die aangeeft of Confirmed is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Confirmed is ingesteld of niet. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Stelt een waarde in voor Cost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Stelt een waarde in voor CostRateTableType.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van CostRateTableType. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Stelt een waarde in voor CostVariance.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Stelt een waarde in voor Created.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Created. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Stelt een waarde in voor Delay.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Stelt een instantie van de ExtendedAttributeCollection‑klasse in voor dit object.

--------------------

Alleen lezen ondersteund voor XML-indeling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | een instantie van de ExtendedAttributeCollection-klasse voor dit object. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Stelt een waarde in voor Finish.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Stelt een waarde in voor FinishVariance.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Stelt een waarde in die aangeeft of FixedMaterial is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of FixedMaterial is ingesteld of niet. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Stelt een waarde in die aangeeft of HasFixedRateUnits is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of HasFixedRateUnits is ingesteld of niet. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Stelt een unieke identifier in voor deze toewijzing.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.UUID | unieke identifier voor deze toewijzing. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Stelt een waarde in voor Hyperlink.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Stelt een waarde in voor HyperlinkAddress.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Stelt een waarde in voor HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Stelt een waarde in voor LevelingDelay.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Stelt een waarde in die aangeeft of LinkedFields is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of LinkedFields is ingesteld of niet. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Stelt eenheden in voor de toewijzing van een materiaalresource met variabele materiaalconsumptie. De variabele materiaalconsumptie betekent dat naarmate de toewijzingsduur verandert, de hoeveelheid gebruikte materialen evenredig verandert.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| eenheden | double | Aantal eenheden opgebouwd in de tijdsperiode. |
|  | rateScaleType | int | Tijdsperiode waarin de eenheidswaarde wordt opgebouwd. |

--------------------

Bijvoorbeeld, om '123/maand' in te stellen, moet SetUnitsScaled(123D, RateScaleType.Month) worden aangeroepen. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Stelt een waarde in die aangeeft of Milestone is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Milestone is ingesteld of niet. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Stelt de tekstnotities in RTF‑formaat in.

--------------------

Alleen ondersteund voor MPP-formaten.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de tekstnotities in RTF-indeling. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Stelt de platte tekst van notities in die uit RTF‑gegevens is gehaald.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | notities' platte tekst geëxtraheerd uit RTF-gegevens. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Stelt een waarde in die aangeeft of Overallocated is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Overallocated is ingesteld of niet. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Stelt een waarde in voor OvertimeCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Stelt een waarde in voor OvertimeWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Stelt een waarde in voor PeakUnits.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Stelt een waarde in voor PercentWorkComplete.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van PercentWorkComplete. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Stelt een waarde in voor RateScale.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van RateScale. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Stelt een waarde in voor RegularWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Stelt een waarde in voor RemainingCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Stelt een waarde in voor RemainingOvertimeCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Stelt een waarde in voor RemainingOvertimeWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Stelt een waarde in voor RemainingWork.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van RemainingWork. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


De resource die aan een taak is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | de aan een taak toegewezen resource. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Stelt een waarde in die aangeeft of ResponsePending is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of ResponsePending is ingesteld of niet. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Stelt een waarde in voor Resume.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Stelt een waarde in voor SV.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Stelt een waarde in voor Start.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Stelt een waarde in voor StartVariance.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Stelt een waarde in voor Stop.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Stelt een waarde in die aangeeft of Summary is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of Summary is ingesteld of niet. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


De taak waaraan een resource is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | de taak waaraan een resource is toegewezen. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Stelt de instantie van de klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) in die elementen van `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) bevat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | de instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse die elementen van `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klasse bevat. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Stelt een waarde van Uid in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Stelt een waarde in voor Units.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Stelt een waarde in die aangeeft of UpdateNeeded is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of UpdateNeeded is ingesteld of niet. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Stelt een waarde in voor VAC.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Stelt een waarde van Work in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Stelt een waarde in voor WorkContour.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Stelt een waarde van WorkVariance in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Splitst taak in twee delen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | Het begin van de werkonderbreking waarop gesplitst moet worden. |
| einde | java.util.Date | Het einde van de werkonderbreking waarop gesplitst moet worden. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | De agenda waarop gesplitst moet worden. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Genereert een lijst met tijdgephaseerde gegevens op basis van de taakduur en de geplande startdatum.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | De agenda waaruit tijdsfasegegevens worden gegenereerd. |

### toString() {#toString--}
```
public String toString()
```


Retourneert een korte tekenreeksrepresentatie van de instantie van de [ResourceAssignment](../../com.aspose.tasks/resourceassignment) klasse. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

**Returns:**
java.lang.String - korte tekenreeks die het toewijzingsobject weergeeft.

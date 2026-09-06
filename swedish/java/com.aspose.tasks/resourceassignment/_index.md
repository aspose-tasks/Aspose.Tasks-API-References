---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en resursallokering i ett projekt."
type: docs
weight: 249
url: /sv/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Representerar en resursallokering i ett projekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returnerar värdet som egenskapen är mappad till i den här behållaren. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [delete()](#delete--) | Tar bort resursuppdrag från projektuppgiftskollektionen. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Returnerar ett värde som indikerar om den här instansen är lika med en specificerad instans av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getACWP()](#getACWP--) | Hämtar ett värde för ACWP. |
| [getActualCost()](#getActualCost--) | Hämtar ett värde för ActualCost. |
| [getActualFinish()](#getActualFinish--) | Hämtar ett värde för ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Hämtar ett värde för ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Hämtar ett värde för ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Hämtar ett värde för ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Hämtar ett värde för ActualStart. |
| [getActualWork()](#getActualWork--) | Hämtar ett värde för ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Hämtar ett värde för ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Hämtar ett värde för AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Hämtar ett värde för AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Hämtar ett värde för BCWP. |
| [getBCWS()](#getBCWS--) | Hämtar ett värde för BCWS. |
| [getBaselines()](#getBaselines--) | Hämtar AssignmentBaselineCollection-objektet. |
| [getBookingType()](#getBookingType--) | Hämtar ett värde för BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Hämtar ett värde för BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Hämtar ett värde för BudgetWork. |
| [getCV()](#getCV--) | Hämtar ett värde för CV. |
| [getConfirmed()](#getConfirmed--) | Hämtar ett värde som indikerar om Confirmed är satt eller inte. |
| [getCost()](#getCost--) | Hämtar ett värde av Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Hämtar ett värde för CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Hämtar ett värde av CostVariance. |
| [getCreated()](#getCreated--) | Hämtar ett värde av Created. |
| [getDelay()](#getDelay--) | Hämtar ett värde för Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Hämtar en instans av klassen ExtendedAttributeCollection för detta objekt. |
| [getFinish()](#getFinish--) | Hämtar ett värde av Finish. |
| [getFinishVariance()](#getFinishVariance--) | Hämtar ett värde för FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Hämtar ett värde som indikerar om FixedMaterial är satt eller inte. |
| [getGuid()](#getGuid--) | Hämtar unikt identifierare för denna tilldelning. |
| [getHyperlink()](#getHyperlink--) | Hämtar ett värde för Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Hämtar ett värde för HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Hämtar ett värde för HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Hämtar ett värde för LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Hämtar ett värde som indikerar om LinkedFields är satt eller inte. |
| [getMilestone()](#getMilestone--) | Hämtar ett värde som indikerar om Milestone är satt eller inte. |
| [getNotesRTF()](#getNotesRTF--) | Hämtar textanteckningarna i RTF-format. |
| [getNotesText()](#getNotesText--) | Hämtar anteckningarnas oformaterade text som extraherats från RTF-data. |
| [getOverallocated()](#getOverallocated--) | Hämtar ett värde som indikerar om Overallocated är satt eller inte. |
| [getOvertimeCost()](#getOvertimeCost--) | Hämtar ett värde för OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Hämtar ett värde för OvertimeWork. |
| [getParentProject()](#getParentProject--) | Hämtar föräldraprojektet för denna tilldelning. |
| [getPeakUnits()](#getPeakUnits--) | Hämtar ett värde för PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Hämtar ett värde för PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Hämtar ett värde för RateScale. |
| [getRegularWork()](#getRegularWork--) | Hämtar ett värde för RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Hämtar ett värde för RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Hämtar ett värde för RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Hämtar ett värde för RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Hämtar ett värde för RemainingWork. |
| [getResource()](#getResource--) | Resursen som är tilldelad en aktivitet. |
| [getResponsePending()](#getResponsePending--) | Hämtar ett värde som indikerar om ResponsePending är satt eller inte. |
| [getResume()](#getResume--) | Hämtar ett värde för Resume. |
| [getSV()](#getSV--) | Hämtar ett värde för SV. |
| [getStart()](#getStart--) | Hämtar ett värde för Start. |
| [getStartVariance()](#getStartVariance--) | Hämtar ett värde för StartVariance. |
| [getStop()](#getStop--) | Hämtar ett värde för Stop. |
| [getSummary()](#getSummary--) | Hämtar ett värde som indikerar om Summary är satt eller inte. |
| [getTask()](#getTask--) | Aktiviteten som en resurs är tilldelad. |
| [getTimephasedData()](#getTimephasedData--) | Hämtar instansen av [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klass som innehåller element av `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klass. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returnerar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objekt med instanser av `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klass inom angivna start- och slutdatum för [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Returnerar instansen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klass som innehåller instanser av `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klass inom angivna start- och slutdatum för den specificerade [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Hämtar mängden tidsfasat arbete för det angivna datum/tidsintervallet. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Hämtar mängden tidsfasat arbete för det angivna datum/tidsintervallet. |
| [getUid()](#getUid--) | Hämtar ett värde för Uid. |
| [getUnits()](#getUnits--) | Hämtar ett värde för Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Hämtar ett värde som indikerar om UpdateNeeded är satt eller inte. |
| [getVAC()](#getVAC--) | Hämtar ett värde för VAC. |
| [getWork()](#getWork--) | Hämtar ett värde för Work. |
| [getWorkContour()](#getWorkContour--) | Hämtar ett värde för WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Hämtar ett värde för WorkVariance. |
| [hasChildren()](#hasChildren--) | Hämtar ett värde som indikerar att denna resursuppgift har underordnade. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Hämtar ett värde som indikerar om HasFixedRateUnits är satt eller inte. |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av [ResourceAssignment](../../com.aspose.tasks/resourceassignment) klass. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Genererar en lista med tidsfasad data. |
| [setACWP(double value)](#setACWP-double-) | Ställer in ett värde för ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Ställer in ett värde för ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Sätter ett värde för ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Sätter ett värde för ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Ställer in ett värde för AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Ställer in ett värde för AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Ställer in ett värde för BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Ställer in ett värde för BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Sätter ett värde för BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Sätter ett värde för BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Sätter ett värde för BudgetWork. |
| [setCV(double value)](#setCV-double-) | Sätter ett värde för CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Sätter ett värde som indikerar om Confirmed är satt eller inte. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sätter ett värde för Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Sätter ett värde för CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Sätter ett värde för CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Sätter ett värde för Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Sätter ett värde för Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Sätter en instans av ExtendedAttributeCollection-klassen för detta objekt. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sätter ett värde för Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Sätter ett värde för FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Sätter ett värde som indikerar om FixedMaterial är satt eller inte. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Sätter ett värde som indikerar om HasFixedRateUnits är satt eller inte. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Sätter en unik identifierare för denna uppgift. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Sätter ett värde för Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Sätter ett värde för HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Sätter ett värde för HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Ställer in ett värde för LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Ställer in ett värde som indikerar om LinkedFields är angivet eller inte. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Ställer in enheter för tilldelning av en materialresurs med variabel materialförbrukning. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Ställer in ett värde som indikerar om Milestone är angivet eller inte. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Ställer in textanteckningarna i RTF-format. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Ställer in anteckningarnas rena text som extraherats från RTF-data. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Ställer in ett värde som anger om Overallocated är satt eller inte. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Ställer in ett värde för PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Ställer in ett värde för PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Ställer in ett värde för RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Ställer in ett värde för RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | Resursen som är tilldelad en aktivitet. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Ställer in ett värde som indikerar om ResponsePending är angivet eller inte. |
| [setResume(Date value)](#setResume-java.util.Date-) | Ställer in ett värde för Resume. |
| [setSV(double value)](#setSV-double-) | Ställer in ett värde för SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ställer in ett värde för Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Ställer in ett värde för StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Ställer in ett värde för Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Ställer in ett värde som indikerar om Summary är angivet eller inte. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | Aktiviteten som en resurs är tilldelad. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ställer in instansen av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) som innehåller element av `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klass. |
| [setUid(int value)](#setUid-int-) | Ställer in ett värde för Uid. |
| [setUnits(double value)](#setUnits-double-) | Ställer in ett värde för Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Ställer in ett värde som indikerar om UpdateNeeded är angivet eller inte. |
| [setVAC(double value)](#setVAC-double-) | Ställer in ett värde för VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ställer in ett värde för Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Ställer in ett värde för WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Ställer in ett värde för WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Delar upp uppgiften i två delar. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Genererar en lista med tidsfasdata baserat på uppgiftens varaktighet och det planerade startdatumet. |
| [toString()](#toString--) | Returnerar en kort strängrepresentation av instansen av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returnerar värdet som egenskapen är mappad till i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Asn](../../com.aspose.tasks/asn) för att hämta egenskapsnyckeln. |

**Returns:**
T - värdet som egenskapen är mappad till i denna behållare.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappar den angivna egenskapen till det angivna värdet i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Asn](../../com.aspose.tasks/asn) för att hämta egenskapsnyckeln. |
| val | T | värdet. |

### delete() {#delete--}
```
public final void delete()
```


Tar bort resursuppdrag från projektuppgiftskollektionen.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Returnerar ett värde som indikerar om den här instansen är lika med en specificerad instans av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Den angivna instansen av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment) för att jämföra med denna instans. |

**Returns:**
boolesk - **True** om den angivna instansen av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment) har samma UID‑värde som denna instans; annars, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Objektet att jämföra med denna instans. |

**Returns:**
boolesk - **True** om o är en ResourceAssignment som tilldelar samma resurs och uppgift som denna instans; annars, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Hämtar ett värde för ACWP.

**Returns:**
double - ett värde av ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Hämtar ett värde för ActualCost.

**Returns:**
java.math.BigDecimal - ett värde av ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Hämtar ett värde för ActualFinish.

**Returns:**
java.util.Date - ett värde för ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Hämtar ett värde för ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - ett värde av ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Hämtar ett värde för ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Hämtar ett värde för ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Hämtar ett värde för ActualStart.

**Returns:**
java.util.Date - ett värde för ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Hämtar ett värde för ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Hämtar ett värde för ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Hämtar ett värde för AssignmentOwner.

**Returns:**
java.lang.String - ett värde av AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Hämtar ett värde för AssignmentOwnerGuid.

**Returns:**
java.lang.String - ett värde av AssignmentOwnerGuid.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Hämtar ett värde för BCWP.

**Returns:**
double - ett värde av BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Hämtar ett värde för BCWS.

**Returns:**
double - ett värde av BCWS.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


Hämtar AssignmentBaselineCollection-objektet. Samlingen av baslinjevärden som är associerade med en tilldelning.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Hämtar ett värde för BookingType.

**Returns:**
int - ett värde av BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Hämtar ett värde för BudgetCost.

**Returns:**
java.math.BigDecimal - ett värde av BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Hämtar ett värde för BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Hämtar ett värde för CV.

**Returns:**
double - ett värde av CV.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Hämtar ett värde som indikerar om Confirmed är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om Confirmed är satt eller inte.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Hämtar ett värde av Cost.

**Returns:**
java.math.BigDecimal - ett värde av Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Hämtar ett värde för CostRateTableType.

**Returns:**
int - ett värde för CostRateTableType.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Hämtar ett värde av CostVariance.

**Returns:**
double - ett värde av CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Hämtar ett värde av Created.

**Returns:**
java.util.Date - ett värde av Created.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Hämtar ett värde för Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Hämtar en instans av klassen ExtendedAttributeCollection för detta objekt.

--------------------

Läsning stöds endast för XML-format.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Hämtar ett värde av Finish.

**Returns:**
java.util.Date - ett värde av Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Hämtar ett värde för FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Hämtar ett värde som indikerar om FixedMaterial är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om FixedMaterial är satt eller inte.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Hämtar unikt identifierare för denna tilldelning.

**Returns:**
java.util.UUID - unik identifierare för denna tilldelning.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hämtar ett värde för Hyperlink.

**Returns:**
java.lang.String - ett värde för Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Hämtar ett värde för HyperlinkAddress.

**Returns:**
java.lang.String - ett värde för HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Hämtar ett värde för HyperlinkSubAddress.

**Returns:**
java.lang.String - ett värde för HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Reserverad för intern användning.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Hämtar ett värde för LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Hämtar ett värde som indikerar om LinkedFields är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om LinkedFields är satt eller inte.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Hämtar ett värde som indikerar om Milestone är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om Milestone är satt eller inte.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Hämtar textanteckningarna i RTF-format.

--------------------

Stöds endast för MPP-format.

**Returns:**
java.lang.String - textanteckningarna i RTF-format.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Hämtar anteckningarnas oformaterade text som extraherats från RTF-data.

**Returns:**
java.lang.String - anteckningarnas rena text extraherad från RTF-data.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Hämtar ett värde som indikerar om Overallocated är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om Overallocated är satt eller inte.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Hämtar ett värde för OvertimeCost.

**Returns:**
java.math.BigDecimal - ett värde av OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Hämtar ett värde för OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldraprojektet för denna tilldelning.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Hämtar ett värde för PeakUnits.

**Returns:**
double - ett värde av PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Hämtar ett värde för PercentWorkComplete.

**Returns:**
int - ett värde av PercentWorkComplete.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Hämtar ett värde för RateScale.

**Returns:**
int - ett värde för RateScale.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Hämtar ett värde för RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Hämtar ett värde för RemainingCost.

**Returns:**
java.math.BigDecimal - ett värde av RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Hämtar ett värde för RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - ett värde av RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Hämtar ett värde för RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Hämtar ett värde för RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


Resursen som är tilldelad en aktivitet.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Hämtar ett värde som indikerar om ResponsePending är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om ResponsePending är satt eller inte.
### getResume() {#getResume--}
```
public final Date getResume()
```


Hämtar ett värde för Resume.

**Returns:**
java.util.Date - ett värde för Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Hämtar ett värde för SV.

**Returns:**
double - ett värde av SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Hämtar ett värde för Start.

**Returns:**
java.util.Date - ett värde av Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Hämtar ett värde för StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Hämtar ett värde för Stop.

**Returns:**
java.util.Date - ett värde för Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Hämtar ett värde som indikerar om Summary är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om Summary är satt eller inte.
### getTask() {#getTask--}
```
public final Task getTask()
```


Aktiviteten som en resurs är tilldelad.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Hämtar instansen av [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klass som innehåller element av `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klass.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returnerar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) objekt med instanser av `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klass inom angivna start- och slutdatum för [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatumet för den tidsfasade datan. |
| slut | java.util.Date | Slutdatumet för den tidsfasade datan. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Returnerar instansen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klass som innehåller instanser av `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) klass inom angivna start- och slutdatum för den specificerade [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatumet för den tidsfasade datan. |
| slut | java.util.Date | Slutdatumet för den tidsfasade datan. |
| timephasedType | byte | Typen av tidsfasade data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Hämtar mängden tidsfasat arbete för det angivna datum/tidsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Starten av datum‑tidsintervallet. |
| slut | java.util.Date | Slutet av datum‑tidsintervallet. |

**Returns:**
double - mängd tidsfasat arbete för det angivna datum‑tidsintervallet.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Hämtar mängden tidsfasat arbete för det angivna datum/tidsintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Starten av datum‑tidsintervallet. |
| slut | java.util.Date | Slutet av datum‑tidsintervallet. |
| timephasedDataType | byte | Typ av den tidsfasade data som ska användas. |

**Returns:**
double - mängd tidsfasat arbete för det angivna datum‑tidsintervallet.
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar ett värde för Uid.

**Returns:**
int - ett värde av Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Hämtar ett värde för Units.

**Returns:**
double - ett värde av Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Hämtar ett värde som indikerar om UpdateNeeded är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om UpdateNeeded är satt eller inte.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Hämtar ett värde för VAC.

**Returns:**
double - ett värde av VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Hämtar ett värde för Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Hämtar ett värde för WorkContour.

**Returns:**
int - ett värde av WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Hämtar ett värde för WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Hämtar ett värde som indikerar att denna resursuppgift har underordnade.

**Returns:**
boolean - Alltid falskt.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Hämtar ett värde som indikerar om HasFixedRateUnits är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om HasFixedRateUnits är satt eller inte.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av [ResourceAssignment](../../com.aspose.tasks/resourceassignment) klass.

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Genererar en lista med tidsfasad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Det angivna startdatumet. |
| tid | double | Den angivna arbetstiden. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Den angivna arbetskalendern. |
| lista | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | Listan med tidsfasade data. |
| isWorking | boolean | Den angivna flaggan som anger om tidsfasade data är aktiva eller inte. |
| typ | int | Den angivna tidsfasade datatypen. |

**Returns:**
java.util.Date - Ett maximalt datum från listan eller startdatum om listan är tom.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Ställer in ett värde för ACWP.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde av ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Ställer in ett värde för ActualCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde av ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Sätter ett värde för ActualFinish.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde av ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Ställer in ett värde för ActualOvertimeCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde av ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Ställer in ett värde för ActualOvertimeWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Ställer in ett värde för ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Sätter ett värde för ActualStart.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde av ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Ställer in ett värde för ActualWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Ställer in ett värde för ActualWorkProtected.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Ställer in ett värde för AssignmentOwner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde av AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Ställer in ett värde för AssignmentOwnerGuid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde av AssignmentOwnerGuid. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Ställer in ett värde för BCWP.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Ställer in ett värde för BCWS.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Sätter ett värde för BookingType.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för BookingType. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Sätter ett värde för BudgetCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Sätter ett värde för BudgetWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Sätter ett värde för CV.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för CV. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Sätter ett värde som indikerar om Confirmed är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Confirmed är satt eller inte. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sätter ett värde för Cost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Sätter ett värde för CostRateTableType.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde av CostRateTableType. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Sätter ett värde för CostVariance.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Sätter ett värde för Created.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Created. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Sätter ett värde för Delay.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Sätter en instans av ExtendedAttributeCollection-klassen för detta objekt.

--------------------

Läsning stöds endast för XML-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | en instans av klassen ExtendedAttributeCollection för detta objekt. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sätter ett värde för Finish.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Sätter ett värde för FinishVariance.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde av FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Sätter ett värde som indikerar om FixedMaterial är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om FixedMaterial är satt eller inte. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Sätter ett värde som indikerar om HasFixedRateUnits är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om HasFixedRateUnits är satt eller inte. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sätter en unik identifierare för denna uppgift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID | unik identifierare för denna tilldelning. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Sätter ett värde för Hyperlink.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Sätter ett värde för HyperlinkAddress.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Sätter ett värde för HyperlinkSubAddress.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Ställer in ett värde för LevelingDelay.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Ställer in ett värde som indikerar om LinkedFields är angivet eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om LinkedFields är satt eller inte. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Ställer in enheter för tilldelning av en materialresurs med variabel materialförbrukning. Den variabla materialförbrukningen betyder att när tilldelningens varaktighet förändras, förändras mängden material som används proportionellt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| enheter | double | Antal enheter som ackumuleras under tidsperioden. |
|  | rateScaleType | int | Tidsperiod då enhetsvärdet ackumuleras. |

--------------------

Till exempel, för att sätta '123/månad', bör SetUnitsScaled(123D, RateScaleType.Month) anropas. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Ställer in ett värde som indikerar om Milestone är angivet eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Milestone är satt eller inte. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Ställer in textanteckningarna i RTF-format.

--------------------

Stöds endast för MPP-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | textanteckningarna i RTF-format. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Ställer in anteckningarnas rena text som extraherats från RTF-data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | anteckningarnas oformaterade text extraherad från RTF-data. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Ställer in ett värde som anger om Overallocated är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Overallocated är satt eller inte. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Ställer in ett värde för OvertimeCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Ställer in ett värde för OvertimeWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Ställer in ett värde för PeakUnits.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Ställer in ett värde för PercentWorkComplete.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för PercentWorkComplete. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Ställer in ett värde för RateScale.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för RateScale. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Ställer in ett värde för RegularWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Ställer in ett värde för RemainingCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Ställer in ett värde för RemainingOvertimeCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Ställer in ett värde för RemainingOvertimeWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Ställer in ett värde för RemainingWork.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för RemainingWork. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


Resursen som är tilldelad en aktivitet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | resursen som är tilldelad en uppgift. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Ställer in ett värde som indikerar om ResponsePending är angivet eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om ResponsePending är satt eller inte. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Ställer in ett värde för Resume.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Ställer in ett värde för SV.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ställer in ett värde för Start.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Ställer in ett värde för StartVariance.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Ställer in ett värde för Stop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Ställer in ett värde som indikerar om Summary är angivet eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om Summary är satt eller inte. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


Aktiviteten som en resurs är tilldelad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | uppgiften som en resurs är tilldelad. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ställer in instansen av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) som innehåller element av `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klass.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | instansen av [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klass som innehåller element av `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) klass. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ställer in ett värde för Uid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Ställer in ett värde för Units.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde av Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Ställer in ett värde som indikerar om UpdateNeeded är angivet eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om UpdateNeeded är satt eller inte. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Ställer in ett värde för VAC.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde av VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ställer in ett värde för Work.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Ställer in ett värde för WorkContour.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde av WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Ställer in ett värde för WorkVariance.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Delar upp uppgiften i två delar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Början av arbetsavbrottet att dela baserat på. |
| slut | java.util.Date | Slutet av arbetsavbrottet att dela baserat på. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Kalendern att dela baserat på. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Genererar en lista med tidsfasdata baserat på uppgiftens varaktighet och det planerade startdatumet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Kalendern att generera tidsfasad data från. |

### toString() {#toString--}
```
public String toString()
```


Returnerar en kort strängrepresentation av instansen av klassen [ResourceAssignment](../../com.aspose.tasks/resourceassignment). De exakta detaljerna för representationen är ospecificerade och kan förändras.

**Returns:**
java.lang.String - kort sträng som representerar tilldelningsobjektet.

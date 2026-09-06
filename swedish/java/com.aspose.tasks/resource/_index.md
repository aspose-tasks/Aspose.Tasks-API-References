---
title: "Resource"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en resurs i ett projekt."
type: docs
weight: 248
url: /sv/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Representerar en resurs i ett projekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Returnerar värdet som egenskapen är mappad till i den här behållaren. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [canLevel()](#canLevel--) | Hämtar ett värde som indikerar om CanLevel är satt eller inte. |
| [delete()](#delete--) | Tar bort en resurs och dess tilldelningar från projektet. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Returnerar ett värde som indikerar om den här instansen är lika med en specificerad instans av klassen [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Returnerar ett värde som anger om detta objekt är lika med ett angivet objekt. |
| [getACWP()](#getACWP--) | Hämtar ett värde för ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Hämtar ett värde för AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Hämtar ett värde för ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Hämtar ett värde för ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Hämtar ett värde för ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Hämtar ett värde för ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Hämtar ett värde för ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Hämtar ett värde för ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Hämtar ett värde för ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Hämtar ett värde för AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Hämtar ett värde för AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Hämtar en samling av resursuppdrag för detta objekt. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Hämtar instansen av klassen [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Hämtar ett värde för AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Hämtar ett värde för AvailableTo. |
| [getBCWP()](#getBCWP--) | Hämtar ett värde för BCWP. |
| [getBCWS()](#getBCWS--) | Hämtar ett värde för BCWS. |
| [getBaselines()](#getBaselines--) | Hämtar en BaselineCollection-instans för detta objekt. |
| [getBookingType()](#getBookingType--) | Hämtar ett värde för BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Hämtar ett värde för BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Hämtar ett värde för BudgetWork. |
| [getCV()](#getCV--) | Hämtar ett värde för CV. |
| [getCalendar()](#getCalendar--) | Hämtar ett värde för Calendar. |
| [getCode()](#getCode--) | Hämtar ett värde av Code. |
| [getCost()](#getCost--) | Hämtar ett värde av Cost. |
| [getCostCenter()](#getCostCenter--) | Hämtar ett värde av CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Hämtar ett värde av CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Hämtar ett värde av CostVariance. |
| [getCreated()](#getCreated--) | Hämtar ett värde av Created. |
| [getEMailAddress()](#getEMailAddress--) | Hämtar ett värde av EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Hämtar värdena för ett utökat attribut. |
| [getFinish()](#getFinish--) | Hämtar ett värde av Finish. |
| [getGroup()](#getGroup--) | Hämtar ett värde av Group. |
| [getGuid()](#getGuid--) | Hämtar ett värde av Guid. |
| [getHyperlink()](#getHyperlink--) | Hämtar titeln eller förklarande text för en hyperlänk som är associerad med en resurs. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Hämtar adressen för en hyperlänk som är associerad med en resurs. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Hämtar den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs. |
| [getId()](#getId--) | Hämtar ett värde av Id. |
| [getInactive()](#getInactive--) | Hämtar ett värde som indikerar om Inactive är satt eller inte. |
| [getInitials()](#getInitials--) | Hämtar ett värde av Initials. |
| [getItems()](#getItems--) | Hämtar underordnade resurser. |
| [getMaterialLabel()](#getMaterialLabel--) | Hämtar ett värde av MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Hämtar ett värde av MaxUnits. |
| [getName()](#getName--) | Hämtar ett värde av Name. |
| [getNotesRTF()](#getNotesRTF--) | Hämtar ett värde av NotesRTF. |
| [getNotesText()](#getNotesText--) | Hämtar ett värde av NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Hämtar ett OutlineCodeCollection-objekt. |
| [getOverallocated()](#getOverallocated--) | Hämtar ett värde som indikerar om Overallocated är satt eller inte. |
| [getOvertimeCost()](#getOvertimeCost--) | Hämtar ett värde för OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Hämtar ett värde för OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Hämtar ett värde för OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Hämtar ett värde för OvertimeWork. |
| [getParentProject()](#getParentProject--) | Hämtar föräldraprojektet för den här containern. |
| [getPeakUnits()](#getPeakUnits--) | Hämtar ett värde för PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Hämtar ett värde för PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Hämtar ett värde för Phonetics. |
| [getRates()](#getRates--) | Hämtar en instans av klassen [RateCollection](../../com.aspose.tasks/ratecollection) för detta objekt. |
| [getRegularWork()](#getRegularWork--) | Hämtar ett värde för RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Hämtar ett värde för RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Hämtar ett värde för RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Hämtar ett värde för RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Hämtar ett värde för RemainingWork. |
| [getSV()](#getSV--) | Hämtar ett värde för SV. |
| [getStandardRate()](#getStandardRate--) | Hämtar ett värde för StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Hämtar ett värde för StandardRateFormat. |
| [getStart()](#getStart--) | Hämtar ett värde för Start. |
| [getTimephasedData()](#getTimephasedData--) | Hämtar en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Returnerar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt med `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) värden inom angivna start- och slutdatum. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Returnerar en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt med `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) värden inom angivna start- och slutdatum för den specificerade [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Hämtar ett värde för Type. |
| [getUid()](#getUid--) | Hämtar ett värde för Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Hämtar ett värde för WindowsUserAccount. |
| [getWork()](#getWork--) | Hämtar ett värde för Work. |
| [getWorkVariance()](#getWorkVariance--) | Hämtar ett värde för WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Hämtar ett värde för Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Returnerar ett hashkodvärde för instansen av klassen [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Hämtar ett värde som indikerar om IsBudget är satt eller inte. |
| [isCostResource()](#isCostResource--) | Hämtar ett värde som indikerar om IsCostResource är satt eller inte. |
| [isEnterprise()](#isEnterprise--) | Hämtar ett värde som indikerar om IsEnterprise är satt eller inte. |
| [isGeneric()](#isGeneric--) | Hämtar ett värde som indikerar om IsGeneric är satt eller inte. |
| [isNull()](#isNull--) | Hämtar ett värde som indikerar om IsNull är satt eller inte. |
| [isRoot()](#isRoot--) | Hämtar flaggan som indikerar om resursen är en rotresurs. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Hämtar ett värde som indikerar om IsTeamAssignmentPool är satt eller inte. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| [setACWP(double value)](#setACWP-double-) | Ställer in ett värde för ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Ställer in ett värde för AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Ställer in ett värde för ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Ställer in ett värde för ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Ställer in ett värde för ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Ställer in ett värde för AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Ställer in ett värde för AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Ställer in ett värde för AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Ställer in ett värde för AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Ställer in ett värde för BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Ställer in ett värde för BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Sätter ett värde för BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om IsBudget är satt eller inte. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Sätter ett värde för BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Sätter ett värde för BudgetWork. |
| [setCV(double value)](#setCV-double-) | Sätter ett värde för CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Sätter ett värde för Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om CanLevel är satt eller inte. |
| [setCode(String value)](#setCode-java.lang.String-) | Sätter ett värde för Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Sätter ett värde för Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Sätter ett värde för CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Sätter ett värde för CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om IsCostResource är satt eller inte. |
| [setCostVariance(double value)](#setCostVariance-double-) | Sätter ett värde för CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Sätter ett värde för Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Sätter ett värde för EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om IsEnterprise är satt eller inte. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Sätter ett värde för Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om IsGeneric är satt eller inte. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Sätter ett värde för Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Sätter ett värde för Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Sätter titeln eller förklarande text för en hyperlänk som är associerad med en resurs. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Sätter adressen för en hyperlänk som är associerad med en resurs. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Sätter den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs. |
| [setId(int value)](#setId-int-) | Sätter ett värde för Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Sätter ett värde som indikerar om Inactive är satt eller inte. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Ställer in ett värde för Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Ställer in ett värde för MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Ställer in ett värde för MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in ett värde för Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Ställer in ett värde för NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Ställer in ett värde för NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om IsNull är satt eller inte. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Ställer in ett värde som anger om Overallocated är satt eller inte. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Ställer in ett värde för OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Ställer in ett värde för OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Ställer in ett värde för PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Ställer in ett värde för PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Ställer in ett värde för Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Ställer in ett värde för RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Ställer in ett värde för RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Ställer in ett värde för RemainingWork. |
| [setSV(double value)](#setSV-double-) | Ställer in ett värde för SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Ställer in ett värde för StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Ställer in ett värde för StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Ställer in ett värde för Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Ställer in ett värde som anger om IsTeamAssignmentPool är satt eller inte. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Ställer in en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt. |
| [setType(int value)](#setType-int-) | Ställer in ett värde för Type. |
| [setUid(int value)](#setUid-int-) | Ställer in ett värde för Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Ställer in ett värde för WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Ställer in ett värde för Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Ställer in ett värde för WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Ställer in ett värde för Workgroup. |
| [toString()](#toString--) | Returnerar en kort strängrepresentation av instansen av klassen [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Returnerar värdet som egenskapen är mappad till i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Rsc](../../com.aspose.tasks/rsc) för att hämta egenskapsnyckeln. |

**Returns:**
T - värdet som egenskapen är mappad till i denna behållare.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Mappar den angivna egenskapen till det angivna värdet i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Rsc](../../com.aspose.tasks/rsc) för att hämta egenskapsnyckeln. |
| val | T | värdet. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Hämtar ett värde som indikerar om CanLevel är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Tar bort en resurs och dess tilldelningar från projektet.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Returnerar ett värde som indikerar om den här instansen är lika med en specificerad instans av klassen [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | Den angivna instansen av klassen [Resource](../../com.aspose.tasks/resource) för att jämföra med denna instans. |

**Returns:**
boolean - **True** om den angivna instansen av klassen [Resource](../../com.aspose.tasks/resource) har samma Uid-värde som denna instans; annars **false**.
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
boolean - **True** om det angivna objektet är en Resource som har samma Uid-värde som denna instans; annars **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Hämtar ett värde för ACWP.

**Returns:**
double - ett värde av ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Hämtar ett värde för AccrueAt.

**Returns:**
int - ett värde av AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Hämtar ett värde för ActiveDirectoryGuid.

**Returns:**
java.lang.String - ett värde av ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Hämtar ett värde för ActualCost.

**Returns:**
java.math.BigDecimal - ett värde av ActualCost.
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Hämtar en samling av resursuppdrag för detta objekt.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Hämtar instansen av klassen [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). Samlingen av perioder då en resurs är tillgänglig.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Hämtar ett värde för AvailableFrom.

**Returns:**
java.util.Date - ett värde av AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Hämtar ett värde för AvailableTo.

**Returns:**
java.util.Date - ett värde av AvailableTo.
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
public final BaselineCollection getBaselines()
```


Hämtar en BaselineCollection-instans för detta objekt. Baslinjevärdena för en resurs.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Hämtar ett värde för Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Hämtar ett värde av Code.

**Returns:**
java.lang.String - ett värde av Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Hämtar ett värde av Cost.

**Returns:**
java.math.BigDecimal - ett värde av Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Hämtar ett värde av CostCenter.

**Returns:**
java.lang.String - ett värde av CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Hämtar ett värde av CostPerUse.

**Returns:**
java.math.BigDecimal - ett värde av CostPerUse.
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Hämtar ett värde av EMailAddress.

**Returns:**
java.lang.String - ett värde av EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Hämtar värdena för ett utökat attribut.

--------------------

Två datadelar är nödvändiga - en pekare tillbaka till den utökade attributtabellen som specificeras antingen med det unika ID:t eller fält-ID:t, och värdet som specificeras antingen med värdet, eller en pekare tillbaka till värdelistan.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Hämtar ett värde av Finish.

**Returns:**
java.util.Date - ett värde av Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Hämtar ett värde av Group.

**Returns:**
java.lang.String - ett värde av Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Hämtar ett värde av Guid.

**Returns:**
java.lang.String - ett värde av Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hämtar titeln eller förklarande text för en hyperlänk som är associerad med en resurs.

**Returns:**
java.lang.String - titeln eller förklarande text för en hyperlänk som är associerad med en resurs.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Hämtar adressen för en hyperlänk som är associerad med en resurs.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

**Returns:**
java.lang.String - adressen för en hyperlänk som är associerad med en resurs.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Hämtar den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

**Returns:**
java.lang.String - den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs.
### getId() {#getId--}
```
public final int getId()
```


Hämtar ett värde av Id.

**Returns:**
int - ett värde av Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Hämtar ett värde som indikerar om Inactive är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Hämtar ett värde av Initials.

**Returns:**
java.lang.String - ett värde av Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Hämtar underordnade resurser.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - underresurser.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Hämtar ett värde av MaterialLabel.

**Returns:**
java.lang.String - ett värde av MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Hämtar ett värde av MaxUnits.

**Returns:**
double - ett värde av MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Hämtar ett värde av Name.

**Returns:**
java.lang.String - ett värde av Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Hämtar ett värde av NotesRTF.

**Returns:**
java.lang.String - ett värde av NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Hämtar ett värde av NotesText.

**Returns:**
java.lang.String - ett värde av NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Hämtar ett OutlineCodeCollection-objekt. Värdet av en konturkod.

--------------------

Två datadelar är nödvändiga - en pekare till outline code-tabellen som specificeras av FieldID, och värdet som specificeras antingen av ValueID eller ValueGUID pekare till värdelistan.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Hämtar ett värde som indikerar om Overallocated är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Hämtar ett värde för OvertimeCost.

**Returns:**
java.math.BigDecimal - ett värde av OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Hämtar ett värde för OvertimeRate.

**Returns:**
java.math.BigDecimal - ett värde av OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Hämtar ett värde för OvertimeRateFormat.

**Returns:**
int - ett värde av OvertimeRateFormat.
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


Hämtar föräldraprojektet för den här containern.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Hämtar ett värde för Phonetics.

**Returns:**
java.lang.String - ett värde av Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Hämtar instansen av [RateCollection](../../com.aspose.tasks/ratecollection)-klassen för detta objekt. Samlingen av perioder och satser som är associerade med varje.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


Hämtar ett värde för SV.

**Returns:**
double - ett värde av SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Hämtar ett värde för StandardRate.

**Returns:**
java.math.BigDecimal - ett värde av StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Hämtar ett värde för StandardRateFormat.

**Returns:**
int - ett värde av StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Hämtar ett värde för Start.

**Returns:**
java.util.Date - ett värde av Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Hämtar en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt.

--------------------

Läsning stöds endast för XML-format.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Returnerar [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt med `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) värden inom angivna start- och slutdatum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatumet för den tidsfasade datan. |
| slut | java.util.Date | Slutdatumet för den tidsfasade datan. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Returnerar en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt med `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) värden inom angivna start- och slutdatum för den specificerade [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| start | java.util.Date | Startdatumet för den tidsfasade datan. |
| slut | java.util.Date | Slutdatumet för den tidsfasade datan. |
| timephasedType | byte | Typen av tidsfasade data ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Hämtar ett värde för Type.

**Returns:**
int - ett värde av Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Hämtar ett värde för Uid.

**Returns:**
int - ett värde av Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Hämtar ett värde för WindowsUserAccount.

**Returns:**
java.lang.String - ett värde av WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Hämtar ett värde för Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Hämtar ett värde för WorkVariance.

**Returns:**
double - ett värde av WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Hämtar ett värde för Workgroup.

**Returns:**
int - ett värde av Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Reserverad för intern användning.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Returnerar ett hashkodvärde för instansen av klassen [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - returnerar ett hash‑kodvärde för detta objekt.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Hämtar ett värde som indikerar om IsBudget är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Hämtar ett värde som indikerar om IsCostResource är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Hämtar ett värde som indikerar om IsEnterprise är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Hämtar ett värde som indikerar om IsGeneric är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Hämtar ett värde som indikerar om IsNull är satt eller inte.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Hämtar flaggan som indikerar om resursen är en rotresurs. Rotresurs är en speciell resurs som är avsedd att stödja intern funktionalitet i MS Projects format och är inte avsedd att användas direkt från användarens kod.

**Returns:**
boolean - flaggan som indikerar om resursen är en rotresurs.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Hämtar ett värde som indikerar om IsTeamAssignmentPool är satt eller inte.

**Returns:**
boolean - ett värde som indikerar om IsTeamAssignmentPool är satt eller inte.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Mappar den angivna egenskapen till det angivna värdet i den här behållaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | den angivna egenskapsnyckeln. [Rsc](../../com.aspose.tasks/rsc) för att hämta egenskapsnyckeln. |
| val | java.util.Date | värdet. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Ställer in ett värde för ACWP.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde av ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Ställer in ett värde för AccrueAt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde av AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Ställer in ett värde för ActiveDirectoryGuid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde av ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Ställer in ett värde för ActualCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde av ActualCost. |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Ställer in ett värde för AvailableFrom.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Ställer in ett värde för AvailableTo.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för AvailableTo. |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Sätter ett värde som indikerar om IsBudget är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om IsBudget är satt eller inte. |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sätter ett värde för Calendar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | ett värde för Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Sätter ett värde som indikerar om CanLevel är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om CanLevel är satt eller inte. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Sätter ett värde för Code.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Sätter ett värde för Cost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Sätter ett värde för CostCenter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Sätter ett värde för CostPerUse.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Sätter ett värde som indikerar om IsCostResource är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om IsCostResource är satt eller inte. |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Sätter ett värde för EMailAddress.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Sätter ett värde som indikerar om IsEnterprise är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om IsEnterprise är satt eller inte. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Sätter ett värde för Finish.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Sätter ett värde som indikerar om IsGeneric är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om IsGeneric är satt eller inte. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Sätter ett värde för Group.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Sätter ett värde för Guid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Sätter titeln eller förklarande text för en hyperlänk som är associerad med en resurs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | titeln eller förklarande texten för en hyperlänk som är associerad med en resurs. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Sätter adressen för en hyperlänk som är associerad med en resurs.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | adressen för en hyperlänk som är associerad med en resurs. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Sätter den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs.

--------------------

Den fullständiga adressen (Hyperlink Href i Microsoft Project) för hyperlänken är en sammanslagning av HyperlinkAddress och HyperlinkSubAddress.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | den specifika platsen i ett dokument i en hyperlänk som är associerad med en resurs. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Sätter ett värde för Id.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Sätter ett värde som indikerar om Inactive är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om Inactive är satt eller inte. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Ställer in ett värde för Initials.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Ställer in ett värde för MaterialLabel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Ställer in ett värde för MaxUnits.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Ställer in ett värde för Name.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Ställer in ett värde för NotesRTF.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Ställer in ett värde för NotesText.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Ställer in ett värde som anger om IsNull är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om IsNull är satt eller inte. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Ställer in ett värde som anger om Overallocated är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ett värde som indikerar om Overallocated är satt eller inte. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Ställer in ett värde för OvertimeCost.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Ställer in ett värde för OvertimeRate.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Ställer in ett värde för OvertimeRateFormat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för OvertimeRateFormat. |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Ställer in ett värde för Phonetics.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för Phonetics. |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Ställer in ett värde för SV.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Ställer in ett värde för StandardRate.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.math.BigDecimal | ett värde för StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Ställer in ett värde för StandardRateFormat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Ställer in ett värde för Start.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date | ett värde för Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Ställer in ett värde som anger om IsTeamAssignmentPool är satt eller inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar om IsTeamAssignmentPool är satt eller inte. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Ställer in en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt.

--------------------

Läsning stöds endast för XML-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | en instans av klassen [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) för detta objekt. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Ställer in ett värde för Type.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Ställer in ett värde för Uid.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Ställer in ett värde för WindowsUserAccount.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | ett värde för WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Ställer in ett värde för Work.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ett värde för Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Ställer in ett värde för WorkVariance.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double | ett värde för WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Ställer in ett värde för Workgroup.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | ett värde för Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Returnerar en kort strängrepresentation av instansen av klassen [Resource](../../com.aspose.tasks/resource). De exakta detaljerna för representationen är ospecificerade och kan förändras.

**Returns:**
java.lang.String – kort sträng som representerar resursobjektet.

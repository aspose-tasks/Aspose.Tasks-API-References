---
title: "Resource"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una risorsa in un progetto."
type: docs
weight: 248
url: /it/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Rappresenta una risorsa in un progetto.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Restituisce il valore a cui la proprietà è mappata in questo contenitore. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [canLevel()](#canLevel--) | Ottiene un valore che indica se CanLevel è impostato o meno. |
| [delete()](#delete--) | Elimina una risorsa e le sue assegnazioni dal progetto. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [getACWP()](#getACWP--) | Ottiene un valore di ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Ottiene un valore di AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Ottiene un valore di ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Ottiene un valore di ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Ottiene un valore di ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Ottiene un valore di ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Ottiene un valore di ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Ottiene un valore di ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Ottiene un valore di ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Ottiene un valore di AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Ottiene un valore di AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Ottiene una collezione di assegnazioni di risorse per questo oggetto. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Ottiene l'istanza della classe [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Ottiene un valore di AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Ottiene un valore di AvailableTo. |
| [getBCWP()](#getBCWP--) | Ottiene un valore di BCWP. |
| [getBCWS()](#getBCWS--) | Ottiene un valore di BCWS. |
| [getBaselines()](#getBaselines--) | Ottiene un'istanza di BaselineCollection per questo oggetto. |
| [getBookingType()](#getBookingType--) | Ottiene un valore di BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Ottiene un valore di BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Ottiene un valore di BudgetWork. |
| [getCV()](#getCV--) | Ottiene un valore di CV. |
| [getCalendar()](#getCalendar--) | Ottiene un valore di Calendar. |
| [getCode()](#getCode--) | Ottiene un valore di Code. |
| [getCost()](#getCost--) | Ottiene un valore di Cost. |
| [getCostCenter()](#getCostCenter--) | Ottiene un valore di CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Ottiene un valore di CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Ottiene un valore di CostVariance. |
| [getCreated()](#getCreated--) | Ottiene un valore di Created. |
| [getEMailAddress()](#getEMailAddress--) | Ottiene un valore di EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Ottiene i valori di un attributo esteso. |
| [getFinish()](#getFinish--) | Ottiene un valore di Finish. |
| [getGroup()](#getGroup--) | Ottiene un valore di Group. |
| [getGuid()](#getGuid--) | Ottiene un valore di Guid. |
| [getHyperlink()](#getHyperlink--) | Ottiene il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Ottiene l'indirizzo di un collegamento ipertestuale associato a una risorsa. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Ottiene la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa. |
| [getId()](#getId--) | Ottiene un valore di Id. |
| [getInactive()](#getInactive--) | Ottiene un valore che indica se Inactive è impostato o meno. |
| [getInitials()](#getInitials--) | Ottiene un valore di Initials. |
| [getItems()](#getItems--) | Ottiene le risorse figlie. |
| [getMaterialLabel()](#getMaterialLabel--) | Ottiene un valore di MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Ottiene un valore di MaxUnits. |
| [getName()](#getName--) | Ottiene un valore di Name. |
| [getNotesRTF()](#getNotesRTF--) | Ottiene un valore di NotesRTF. |
| [getNotesText()](#getNotesText--) | Ottiene un valore di NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Ottiene un oggetto OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | Ottiene un valore che indica se Overallocated è impostato o meno. |
| [getOvertimeCost()](#getOvertimeCost--) | Ottiene un valore di OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Ottiene un valore di OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Ottiene un valore di OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Ottiene un valore di OvertimeWork. |
| [getParentProject()](#getParentProject--) | Ottiene il progetto genitore per questo contenitore. |
| [getPeakUnits()](#getPeakUnits--) | Ottiene un valore di PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Ottiene un valore di PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Ottiene un valore di Phonetics. |
| [getRates()](#getRates--) | Ottiene l'istanza della classe [RateCollection](../../com.aspose.tasks/ratecollection) per questo oggetto. |
| [getRegularWork()](#getRegularWork--) | Ottiene un valore di RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Ottiene un valore di RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Ottiene un valore di RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Ottiene un valore di RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Ottiene un valore di RemainingWork. |
| [getSV()](#getSV--) | Ottiene un valore di SV. |
| [getStandardRate()](#getStandardRate--) | Ottiene un valore di StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Ottiene un valore di StandardRateFormat. |
| [getStart()](#getStart--) | Ottiene un valore di Start. |
| [getTimephasedData()](#getTimephasedData--) | Ottiene un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Restituisce [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto con i valori `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) entro le date di inizio e fine specificate. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Restituisce un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto con i valori `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) entro le date di inizio e fine specificate del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) indicato. |
| [getType()](#getType--) | Ottiene un valore di Type. |
| [getUid()](#getUid--) | Ottiene un valore di Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Ottiene un valore di WindowsUserAccount. |
| [getWork()](#getWork--) | Ottiene un valore di Work. |
| [getWorkVariance()](#getWorkVariance--) | Ottiene un valore di WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Ottiene un valore di Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Restituisce un valore di codice hash per l'istanza della classe [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Ottiene un valore che indica se IsBudget è impostato o meno. |
| [isCostResource()](#isCostResource--) | Ottiene un valore che indica se IsCostResource è impostato o meno. |
| [isEnterprise()](#isEnterprise--) | Ottiene un valore che indica se IsEnterprise è impostato o meno. |
| [isGeneric()](#isGeneric--) | Ottiene un valore che indica se IsGeneric è impostato o meno. |
| [isNull()](#isNull--) | Ottiene un valore che indica se IsNull è impostato o meno. |
| [isRoot()](#isRoot--) | Ottiene il flag che indica se la risorsa è una risorsa radice. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Ottiene un valore che indica se IsTeamAssignmentPool è impostato o meno. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappa la proprietà specificata al valore specificato in questo contenitore. |
| [setACWP(double value)](#setACWP-double-) | Imposta un valore di ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Imposta un valore di AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Imposta un valore di ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Imposta un valore di ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Imposta un valore di ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Imposta un valore di ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Imposta un valore di ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Imposta un valore di ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Imposta un valore di AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Imposta un valore di AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Imposta un valore di AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Imposta un valore di AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Imposta un valore di BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Imposta un valore di BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Imposta un valore di BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se IsBudget è impostato o meno. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Imposta un valore di BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Imposta un valore di BudgetWork. |
| [setCV(double value)](#setCV-double-) | Imposta un valore di CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Imposta un valore di Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se CanLevel è impostato o meno. |
| [setCode(String value)](#setCode-java.lang.String-) | Imposta un valore di Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Imposta un valore di Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Imposta un valore di CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Imposta un valore di CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se IsCostResource è impostato o meno. |
| [setCostVariance(double value)](#setCostVariance-double-) | Imposta un valore di CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Imposta un valore di Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Imposta un valore di EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se IsEnterprise è impostato o meno. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Imposta un valore di Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se IsGeneric è impostato o meno. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Imposta un valore di Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Imposta un valore di Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Imposta il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Imposta l'indirizzo di un collegamento ipertestuale associato a una risorsa. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Imposta la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa. |
| [setId(int value)](#setId-int-) | Imposta un valore di Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se Inactive è impostato o meno. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Imposta un valore di Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Imposta un valore di MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Imposta un valore di MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Imposta un valore di Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Imposta un valore di NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Imposta un valore di NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se IsNull è impostato o meno. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Imposta un valore che indica se Overallocated è impostato o meno. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Imposta un valore di OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Imposta un valore di OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Imposta un valore di OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Imposta un valore di PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Imposta un valore di PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Imposta un valore di Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Imposta un valore di RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Imposta un valore di RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Imposta un valore di RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Imposta un valore di RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Imposta un valore di RemainingWork. |
| [setSV(double value)](#setSV-double-) | Imposta un valore di SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Imposta un valore di StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Imposta un valore di StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Imposta un valore di Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Imposta un valore che indica se IsTeamAssignmentPool è impostato o meno. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Imposta un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto. |
| [setType(int value)](#setType-int-) | Imposta un valore di Type. |
| [setUid(int value)](#setUid-int-) | Imposta un valore di Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Imposta un valore di WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Imposta un valore di Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Imposta un valore di WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Imposta un valore di Workgroup. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa breve dell'istanza della classe [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Restituisce il valore a cui la proprietà è mappata in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Rsc](../../com.aspose.tasks/rsc) per ottenere la chiave della proprietà. |

**Returns:**
T - il valore a cui la proprietà è mappata in questo contenitore.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Mappa la proprietà specificata al valore specificato in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la chiave della proprietà specificata. [Rsc](../../com.aspose.tasks/rsc) per ottenere la chiave della proprietà. |
| val | T | il valore. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Ottiene un valore che indica se CanLevel è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Elimina una risorsa e le sue assegnazioni dal progetto.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | L'istanza specificata della classe [Resource](../../com.aspose.tasks/resource) da confrontare con questa istanza. |

**Returns:**
boolean - **True** se l'istanza specificata della classe [Resource](../../com.aspose.tasks/resource) ha lo stesso valore Uid di questa istanza; altrimenti, **false**.
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
boolean - **True** se l'oggetto specificato è una Resource che ha lo stesso valore Uid di questa istanza; altrimenti, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Ottiene un valore di ACWP.

**Returns:**
double - un valore di ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Ottiene un valore di AccrueAt.

**Returns:**
int - un valore di AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Ottiene un valore di ActiveDirectoryGuid.

**Returns:**
java.lang.String - un valore di ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Ottiene un valore di ActualCost.

**Returns:**
java.math.BigDecimal - un valore di ActualCost.
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Ottiene una collezione di assegnazioni di risorse per questo oggetto.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Ottiene l'istanza della classe [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). La collezione di periodi durante i quali una risorsa è disponibile.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Ottiene un valore di AvailableFrom.

**Returns:**
java.util.Date - un valore di AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Ottiene un valore di AvailableTo.

**Returns:**
java.util.Date - un valore di AvailableTo.
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
public final BaselineCollection getBaselines()
```


Ottiene un'istanza di BaselineCollection per questo oggetto. I valori di baseline per una risorsa.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Ottiene un valore di Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Ottiene un valore di Code.

**Returns:**
java.lang.String - un valore di Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ottiene un valore di Cost.

**Returns:**
java.math.BigDecimal - un valore di Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Ottiene un valore di CostCenter.

**Returns:**
java.lang.String - un valore di CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Ottiene un valore di CostPerUse.

**Returns:**
java.math.BigDecimal - un valore di CostPerUse.
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Ottiene un valore di EMailAddress.

**Returns:**
java.lang.String - un valore di EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Ottiene i valori di un attributo esteso.

--------------------

Sono necessari due elementi di dati - un puntatore alla tabella degli attributi estesi specificata sia dall'ID univoco sia dal Field ID, e il valore specificato sia con il valore, sia con un puntatore alla lista dei valori.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ottiene un valore di Finish.

**Returns:**
java.util.Date - un valore di Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Ottiene un valore di Group.

**Returns:**
java.lang.String - un valore di Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Ottiene un valore di Guid.

**Returns:**
java.lang.String - un valore di Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Ottiene il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa.

**Returns:**
java.lang.String - il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Ottiene l'indirizzo di un collegamento ipertestuale associato a una risorsa.

--------------------

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

**Returns:**
java.lang.String - l'indirizzo per un collegamento ipertestuale associato a una risorsa.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Ottiene la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa.

--------------------

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

**Returns:**
java.lang.String - la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa.
### getId() {#getId--}
```
public final int getId()
```


Ottiene un valore di Id.

**Returns:**
int - un valore di Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Ottiene un valore che indica se Inactive è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Ottiene un valore di Initials.

**Returns:**
java.lang.String - un valore di Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Ottiene le risorse figlie.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - risorse figlie.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Ottiene un valore di MaterialLabel.

**Returns:**
java.lang.String - un valore di MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Ottiene un valore di MaxUnits.

**Returns:**
double - un valore di MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Ottiene un valore di Name.

**Returns:**
java.lang.String - un valore di Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Ottiene un valore di NotesRTF.

**Returns:**
java.lang.String - un valore di NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Ottiene un valore di NotesText.

**Returns:**
java.lang.String - un valore di NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Ottiene un oggetto OutlineCodeCollection. Il valore di un codice di struttura.

--------------------

Sono necessari due dati - un puntatore alla tabella dei codici di struttura specificata dal FieldID, e il valore specificato sia dal puntatore ValueID sia dal puntatore ValueGUID all'elenco dei valori.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Ottiene un valore che indica se Overallocated è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Ottiene un valore di OvertimeCost.

**Returns:**
java.math.BigDecimal - un valore di OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Ottiene un valore di OvertimeRate.

**Returns:**
java.math.BigDecimal - un valore di OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Ottiene un valore di OvertimeRateFormat.

**Returns:**
int - un valore di OvertimeRateFormat.
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


Ottiene il progetto genitore per questo contenitore.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Ottiene un valore di Phonetics.

**Returns:**
java.lang.String - un valore di Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Ottiene l'istanza della classe [RateCollection](../../com.aspose.tasks/ratecollection) per questo oggetto. La raccolta di periodi e tariffe associate a ciascuno.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


Ottiene un valore di SV.

**Returns:**
double - un valore di SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Ottiene un valore di StandardRate.

**Returns:**
java.math.BigDecimal - un valore di StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Ottiene un valore di StandardRateFormat.

**Returns:**
int - un valore di StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Ottiene un valore di Start.

**Returns:**
java.util.Date - un valore di Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Ottiene un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto.

--------------------

Lettura supportata solo per il formato XML.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Restituisce [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto con i valori `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) entro le date di inizio e fine specificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | La data di inizio per i dati a intervallo temporale. |
| fine | java.util.Date | La data di fine per i dati a intervalli temporali. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Restituisce un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto con i valori `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) entro le date di inizio e fine specificate del [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) indicato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | java.util.Date | La data di inizio per i dati a intervalli temporali. |
| fine | java.util.Date | La data di fine per i dati a intervalli temporali. |
| timephasedType | byte | Il tipo di dati a intervalli temporali ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Ottiene un valore di Type.

**Returns:**
int - un valore di Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Ottiene un valore di Uid.

**Returns:**
int - un valore di Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Ottiene un valore di WindowsUserAccount.

**Returns:**
java.lang.String - un valore di WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ottiene un valore di Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Ottiene un valore di WorkVariance.

**Returns:**
double - un valore di WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Ottiene un valore di Workgroup.

**Returns:**
int - un valore di Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Riservato per uso interno.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Restituisce un valore di codice hash per l'istanza della classe [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - restituisce un valore di codice hash per questo oggetto.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Ottiene un valore che indica se IsBudget è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Ottiene un valore che indica se IsCostResource è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Ottiene un valore che indica se IsEnterprise è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Ottiene un valore che indica se IsGeneric è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Ottiene un valore che indica se IsNull è impostato o meno.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Restituisce il flag che indica se la risorsa è una risorsa radice. La risorsa radice è una risorsa speciale destinata a supportare gli aspetti interni dei formati di MS Project e non è destinata a essere utilizzata direttamente dal codice dell'utente.

**Returns:**
boolean - il flag che indica se la risorsa è una risorsa radice.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Ottiene un valore che indica se IsTeamAssignmentPool è impostato o meno.

**Returns:**
boolean - un valore che indica se IsTeamAssignmentPool è impostato o meno.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Mappa la proprietà specificata al valore specificato in questo contenitore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | la chiave della proprietà specificata. [Rsc](../../com.aspose.tasks/rsc) per ottenere la chiave della proprietà. |
| val | java.util.Date | il valore. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Imposta un valore di ACWP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Imposta un valore di AccrueAt.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Imposta un valore di ActiveDirectoryGuid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Imposta un valore di ActualCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di ActualCost. |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Imposta un valore di AvailableFrom.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Imposta un valore di AvailableTo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di AvailableTo. |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Imposta un valore che indica se IsBudget è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se IsBudget è impostato o meno. |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Imposta un valore di Calendar.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | un valore di Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Imposta un valore che indica se CanLevel è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se CanLevel è impostato o meno. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Imposta un valore di Code.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Imposta un valore di Cost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Imposta un valore di CostCenter.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Imposta un valore di CostPerUse.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Imposta un valore che indica se IsCostResource è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se IsCostResource è impostato o meno. |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Imposta un valore di EMailAddress.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Imposta un valore che indica se IsEnterprise è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se IsEnterprise è impostato o meno. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Imposta un valore di Finish.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Imposta un valore che indica se IsGeneric è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se IsGeneric è impostato o meno. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Imposta un valore di Group.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Imposta un valore di Guid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Imposta il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | il titolo o il testo esplicativo di un collegamento ipertestuale associato a una risorsa. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Imposta l'indirizzo di un collegamento ipertestuale associato a una risorsa.

--------------------

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | l'indirizzo per un collegamento ipertestuale associato a una risorsa. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Imposta la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa.

--------------------

L'indirizzo completo (Hyperlink Href in Microsoft Project) del collegamento ipertestuale è una concatenazione di HyperlinkAddress e HyperlinkSubAddress.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | la posizione specifica in un documento in un collegamento ipertestuale associato a una risorsa. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Imposta un valore di Id.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Imposta un valore che indica se Inactive è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se Inactive è impostato o meno. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Imposta un valore di Initials.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Imposta un valore di MaterialLabel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Imposta un valore di MaxUnits.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Imposta un valore di Name.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Imposta un valore di NotesRTF.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Imposta un valore di NotesText.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Imposta un valore che indica se IsNull è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se IsNull è impostato o meno. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Imposta un valore che indica se Overallocated è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | un valore che indica se Overallocated è impostato o meno. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Imposta un valore di OvertimeCost.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Imposta un valore di OvertimeRate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Imposta un valore di OvertimeRateFormat.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di OvertimeRateFormat. |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Imposta un valore di Phonetics.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di Phonetics. |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Imposta un valore di SV.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Imposta un valore di StandardRate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.math.BigDecimal | un valore di StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Imposta un valore di StandardRateFormat.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Imposta un valore di Start.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | un valore di Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Imposta un valore che indica se IsTeamAssignmentPool è impostato o meno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | un valore che indica se IsTeamAssignmentPool è impostato o meno. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Imposta un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto.

--------------------

Lettura supportata solo per il formato XML.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | un'istanza della classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) per questo oggetto. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Imposta un valore di Type.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Imposta un valore di Uid.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Imposta un valore di WindowsUserAccount.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | un valore di WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Imposta un valore di Work.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | un valore di Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Imposta un valore di WorkVariance.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double | un valore di WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Imposta un valore di Workgroup.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | un valore di Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione in forma di stringa breve dell'istanza della classe [Resource](../../com.aspose.tasks/resource). I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche.

**Returns:**
java.lang.String - stringa breve che rappresenta l'oggetto risorsa.

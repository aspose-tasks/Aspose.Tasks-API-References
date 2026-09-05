---
title: "Resource"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een resource in een project voor."
type: docs
weight: 248
url: /nl/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Stelt een resource in een project voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Retourneert de waarde waaraan de eigenschap in deze container is toegewezen. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [canLevel()](#canLevel--) | Haalt een waarde op die aangeeft of CanLevel is ingesteld of niet. |
| [delete()](#delete--) | Verwijdert een resource en de bijbehorende toewijzingen uit het project. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [Resource](../../com.aspose.tasks/resource) klasse. |
| [equals(Object obj)](#equals-java.lang.Object-) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [getACWP()](#getACWP--) | Haalt een waarde van ACWP op. |
| [getAccrueAt()](#getAccrueAt--) | Haalt een waarde van AccrueAt op. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Haalt een waarde van ActiveDirectoryGuid op. |
| [getActualCost()](#getActualCost--) | Haalt een waarde van ActualCost op. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Haalt een waarde van ActualOvertimeCost op. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Haalt een waarde van ActualOvertimeWork op. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Haalt een waarde van ActualOvertimeWorkProtected op. |
| [getActualWork()](#getActualWork--) | Haalt een waarde van ActualWork op. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Haalt een waarde van ActualWorkProtected op. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Haalt een waarde van AssignmentOwner op. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Haalt een waarde van AssignmentOwnerGuid op. |
| [getAssignments()](#getAssignments--) | Haalt een collectie van resource-toewijzingen voor dit object op. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Haalt de instantie van de [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) klasse op. |
| [getAvailableFrom()](#getAvailableFrom--) | Haalt een waarde van AvailableFrom op. |
| [getAvailableTo()](#getAvailableTo--) | Haalt een waarde van AvailableTo op. |
| [getBCWP()](#getBCWP--) | Haalt een waarde van BCWP op. |
| [getBCWS()](#getBCWS--) | Haalt een waarde van BCWS op. |
| [getBaselines()](#getBaselines--) | Haalt een BaselineCollection‑instantie voor dit object op. |
| [getBookingType()](#getBookingType--) | Haalt een waarde van BookingType op. |
| [getBudgetCost()](#getBudgetCost--) | Haalt een waarde van BudgetCost op. |
| [getBudgetWork()](#getBudgetWork--) | Haalt een waarde van BudgetWork op. |
| [getCV()](#getCV--) | Haalt een waarde van CV op. |
| [getCalendar()](#getCalendar--) | Haalt een waarde van Calendar op. |
| [getCode()](#getCode--) | Haalt een waarde van Code op. |
| [getCost()](#getCost--) | Haalt een waarde van Cost op. |
| [getCostCenter()](#getCostCenter--) | Haalt een waarde van CostCenter op. |
| [getCostPerUse()](#getCostPerUse--) | Haalt een waarde van CostPerUse op. |
| [getCostVariance()](#getCostVariance--) | Haalt een waarde van CostVariance op. |
| [getCreated()](#getCreated--) | Haalt een waarde van Created op. |
| [getEMailAddress()](#getEMailAddress--) | Haalt een waarde van EMailAddress op. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Haalt de waarden van een uitgebreid attribuut op. |
| [getFinish()](#getFinish--) | Haalt een waarde van Finish op. |
| [getGroup()](#getGroup--) | Haalt een waarde van Group op. |
| [getGuid()](#getGuid--) | Haalt een waarde van Guid op. |
| [getHyperlink()](#getHyperlink--) | Haalt de titel of de toelichtende tekst van een hyperlink die aan een resource is gekoppeld op. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Haalt het adres van een hyperlink die aan een resource is gekoppeld op. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Haalt de specifieke locatie in een document in een hyperlink die aan een resource is gekoppeld op. |
| [getId()](#getId--) | Haalt een waarde van Id op. |
| [getInactive()](#getInactive--) | Haalt een waarde op die aangeeft of Inactive is ingesteld of niet. |
| [getInitials()](#getInitials--) | Haalt een waarde van Initials op. |
| [getItems()](#getItems--) | Haalt onderliggende resources op. |
| [getMaterialLabel()](#getMaterialLabel--) | Haalt een waarde van MaterialLabel op. |
| [getMaxUnits()](#getMaxUnits--) | Haalt een waarde van MaxUnits op. |
| [getName()](#getName--) | Haalt een waarde van Name op. |
| [getNotesRTF()](#getNotesRTF--) | Haalt een waarde van NotesRTF op. |
| [getNotesText()](#getNotesText--) | Haalt een waarde van NotesText op. |
| [getOutlineCode()](#getOutlineCode--) | Haalt een OutlineCodeCollection-object op. |
| [getOverallocated()](#getOverallocated--) | Haalt een waarde op die aangeeft of Overallocated is ingesteld of niet. |
| [getOvertimeCost()](#getOvertimeCost--) | Haalt een waarde op van OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Haalt een waarde op van OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Haalt een waarde op van OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Haalt een waarde op van OvertimeWork. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op voor deze container. |
| [getPeakUnits()](#getPeakUnits--) | Haalt een waarde op van PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Haalt een waarde op van PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Haalt een waarde op van Phonetics. |
| [getRates()](#getRates--) | Haalt een instantie op van de [RateCollection](../../com.aspose.tasks/ratecollection) klasse voor dit object. |
| [getRegularWork()](#getRegularWork--) | Haalt een waarde op van RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Haalt een waarde op van RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Haalt een waarde op van RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Haalt een waarde op van RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Haalt een waarde op van RemainingWork. |
| [getSV()](#getSV--) | Haalt een waarde op van SV. |
| [getStandardRate()](#getStandardRate--) | Haalt een waarde op van StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Haalt een waarde op van StandardRateFormat. |
| [getStart()](#getStart--) | Haalt een waarde op van Start. |
| [getTimephasedData()](#getTimephasedData--) | Haalt een instantie op van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse voor dit object. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Retourneert [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) voor dit object met `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) waarden binnen de opgegeven start- en einddatums. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Retourneert een instantie van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse voor dit object met de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) waarden binnen de opgegeven start- en einddatums van het gespecificeerde [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Haalt een waarde op van Type. |
| [getUid()](#getUid--) | Haalt een waarde op van Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Haalt een waarde op van WindowsUserAccount. |
| [getWork()](#getWork--) | Haalt een waarde op van Work. |
| [getWorkVariance()](#getWorkVariance--) | Haalt een waarde op van WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Haalt een waarde op van Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Retourneert een hashcode-waarde voor de instantie van de [Resource](../../com.aspose.tasks/resource) klasse. |
| [isBudget()](#isBudget--) | Haalt een waarde op die aangeeft of IsBudget is ingesteld of niet. |
| [isCostResource()](#isCostResource--) | Haalt een waarde op die aangeeft of IsCostResource is ingesteld of niet. |
| [isEnterprise()](#isEnterprise--) | Haalt een waarde op die aangeeft of IsEnterprise is ingesteld of niet. |
| [isGeneric()](#isGeneric--) | Haalt een waarde op die aangeeft of IsGeneric is ingesteld of niet. |
| [isNull()](#isNull--) | Haalt een waarde op die aangeeft of IsNull is ingesteld of niet. |
| [isRoot()](#isRoot--) | Haalt de vlag op die aangeeft of de resource een rootresource is. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Haalt een waarde op die aangeeft of IsTeamAssignmentPool is ingesteld of niet. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container. |
| [setACWP(double value)](#setACWP-double-) | Stelt een waarde in voor ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Stelt een waarde in voor AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Stelt een waarde in voor ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Stelt een waarde in voor ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Stelt een waarde in voor ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Stelt een waarde in voor AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Stelt een waarde in voor AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Stelt een waarde in voor AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Stelt een waarde in voor AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Stelt een waarde in voor BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Stelt een waarde in voor BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Stelt een waarde in voor BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of IsBudget is ingesteld of niet. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Stelt een waarde in voor BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor BudgetWork. |
| [setCV(double value)](#setCV-double-) | Stelt een waarde in voor CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Stelt een waarde in voor Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of CanLevel is ingesteld of niet. |
| [setCode(String value)](#setCode-java.lang.String-) | Stelt een waarde in voor Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Stelt een waarde in voor Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Stelt een waarde in voor CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Stelt een waarde in voor CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of IsCostResource is ingesteld of niet. |
| [setCostVariance(double value)](#setCostVariance-double-) | Stelt een waarde in voor CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Stelt een waarde in voor Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Stelt een waarde in voor EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of IsEnterprise is ingesteld of niet. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Stelt een waarde in voor Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of IsGeneric is ingesteld of niet. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Stelt een waarde in voor Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Stelt een waarde in voor Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Stelt de titel of verklarende tekst van een hyperlink die aan een resource is gekoppeld in. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Stelt het adres in voor een hyperlink die aan een resource is gekoppeld. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Stelt de specifieke locatie in een document in voor een hyperlink die aan een resource is gekoppeld. |
| [setId(int value)](#setId-int-) | Stelt een waarde in voor Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of Inactive is ingesteld of niet. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Stelt een waarde in voor Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Stelt een waarde in voor MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Stelt een waarde in voor MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Stelt een waarde in voor Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Stelt een waarde in voor NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Stelt een waarde in voor NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of IsNull is ingesteld of niet. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Stelt een waarde in die aangeeft of Overallocated is ingesteld of niet. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Stelt een waarde in voor OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Stelt een waarde in voor OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Stelt een waarde in voor PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Stelt een waarde in voor PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Stelt een waarde in voor Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Stelt een waarde in voor RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Stelt een waarde in voor RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Stelt een waarde in voor RemainingWork. |
| [setSV(double value)](#setSV-double-) | Stelt een waarde in voor SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Stelt een waarde in voor StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Stelt een waarde in voor StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Stelt een waarde in voor Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Stelt een waarde in die aangeeft of IsTeamAssignmentPool is ingesteld of niet. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Stelt een instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse in voor dit object. |
| [setType(int value)](#setType-int-) | Stelt een waarde van Type in. |
| [setUid(int value)](#setUid-int-) | Stelt een waarde van Uid in. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Stelt een waarde van WindowsUserAccount in. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Stelt een waarde van Work in. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Stelt een waarde van WorkVariance in. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Stelt een waarde van Workgroup in. |
| [toString()](#toString--) | Retourneert een korte tekenreeksrepresentatie van de instantie van de [Resource](../../com.aspose.tasks/resource) klasse. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Retourneert de waarde waaraan de eigenschap in deze container is toegewezen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Rsc](../../com.aspose.tasks/rsc) voor het verkrijgen van de eigenschapssleutel. |

**Returns:**
T - de waarde waaraan de eigenschap in deze container is toegewezen.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Rsc](../../com.aspose.tasks/rsc) voor het verkrijgen van de eigenschapssleutel. |
| val | T | de waarde. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Haalt een waarde op die aangeeft of CanLevel is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Verwijdert een resource en de bijbehorende toewijzingen uit het project.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven instantie van de [Resource](../../com.aspose.tasks/resource) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | De opgegeven instantie van de [Resource](../../com.aspose.tasks/resource) klasse om te vergelijken met deze instantie. |

**Returns:**
boolean - **True** als de opgegeven instantie van de [Resource](../../com.aspose.tasks/resource) klasse dezelfde Uid-waarde heeft als deze instantie; anders, **false**.
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
boolean - **True** als het opgegeven object een Resource is die dezelfde Uid-waarde heeft als deze instantie; anders, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Haalt een waarde van ACWP op.

**Returns:**
double - een waarde van ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Haalt een waarde van AccrueAt op.

**Returns:**
int - een waarde van AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Haalt een waarde van ActiveDirectoryGuid op.

**Returns:**
java.lang.String - een waarde van ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Haalt een waarde van ActualCost op.

**Returns:**
java.math.BigDecimal - een waarde van ActualCost.
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Haalt een collectie van resource-toewijzingen voor dit object op.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Haalt de instantie van de [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) klasse op. De verzameling perioden waarin een resource beschikbaar is.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Haalt een waarde van AvailableFrom op.

**Returns:**
java.util.Date - een waarde van AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Haalt een waarde van AvailableTo op.

**Returns:**
java.util.Date - een waarde van AvailableTo.
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
public final BaselineCollection getBaselines()
```


Haalt een BaselineCollection‑instantie op voor dit object. De baseline‑waarden voor een resource.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Haalt een waarde van Calendar op.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Haalt een waarde van Code op.

**Returns:**
java.lang.String - een waarde van Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Haalt een waarde van Cost op.

**Returns:**
java.math.BigDecimal - een waarde van Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Haalt een waarde van CostCenter op.

**Returns:**
java.lang.String - een waarde van CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Haalt een waarde van CostPerUse op.

**Returns:**
java.math.BigDecimal - een waarde van CostPerUse.
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Haalt een waarde van EMailAddress op.

**Returns:**
java.lang.String - een waarde van EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Haalt de waarden van een uitgebreid attribuut op.

--------------------

Twee gegevensstukken zijn nodig - een verwijzing terug naar de uitgebreide attribuuttabel die wordt gespecificeerd door de unieke ID of de Field ID, en de waarde die wordt gespecificeerd met de waarde, of een verwijzing terug naar de waardelijst.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Haalt een waarde van Finish op.

**Returns:**
java.util.Date - een waarde van Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Haalt een waarde van Group op.

**Returns:**
java.lang.String - een waarde van Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Haalt een waarde van Guid op.

**Returns:**
java.lang.String - een waarde van Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Haalt de titel of de toelichtende tekst van een hyperlink die aan een resource is gekoppeld op.

**Returns:**
java.lang.String - de titel of verklarende tekst van een hyperlink die aan een resource is gekoppeld.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Haalt het adres van een hyperlink die aan een resource is gekoppeld op.

--------------------

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

**Returns:**
java.lang.String - het adres voor een hyperlink die aan een resource is gekoppeld.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Haalt de specifieke locatie in een document in een hyperlink die aan een resource is gekoppeld op.

--------------------

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

**Returns:**
java.lang.String - de specifieke locatie in een document in een hyperlink die aan een resource is gekoppeld.
### getId() {#getId--}
```
public final int getId()
```


Haalt een waarde van Id op.

**Returns:**
int - een waarde van Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Haalt een waarde op die aangeeft of Inactive is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Haalt een waarde van Initials op.

**Returns:**
java.lang.String - een waarde van Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Haalt onderliggende resources op.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - onderliggende resources.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Haalt een waarde van MaterialLabel op.

**Returns:**
java.lang.String - een waarde van MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Haalt een waarde van MaxUnits op.

**Returns:**
double - een waarde van MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Haalt een waarde van Name op.

**Returns:**
java.lang.String - een waarde van Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Haalt een waarde van NotesRTF op.

**Returns:**
java.lang.String - een waarde van NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Haalt een waarde van NotesText op.

**Returns:**
java.lang.String - een waarde van NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Haalt een OutlineCodeCollection-object op. De waarde van een outlinecode.

--------------------

Twee gegevensstukken zijn nodig - een verwijzing naar de outline code-tabel die wordt gespecificeerd door de FieldID, en de waarde die wordt gespecificeerd door ofwel de ValueID of de ValueGUID-verwijzing naar de waardelijst.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Haalt een waarde op die aangeeft of Overallocated is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Haalt een waarde op van OvertimeCost.

**Returns:**
java.math.BigDecimal - een waarde van OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Haalt een waarde op van OvertimeRate.

**Returns:**
java.math.BigDecimal - een waarde van OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Haalt een waarde op van OvertimeRateFormat.

**Returns:**
int - een waarde van OvertimeRateFormat.
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


Haalt het bovenliggende project op voor deze container.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Haalt een waarde op van Phonetics.

**Returns:**
java.lang.String - een waarde van Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Haalt de instantie van de [RateCollection](../../com.aspose.tasks/ratecollection)-klasse voor dit object op. De verzameling van perioden en tarieven die aan elk ervan zijn gekoppeld.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


Haalt een waarde op van SV.

**Returns:**
double - een waarde van SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Haalt een waarde op van StandardRate.

**Returns:**
java.math.BigDecimal - een waarde van StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Haalt een waarde op van StandardRateFormat.

**Returns:**
int - een waarde van StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Haalt een waarde op van Start.

**Returns:**
java.util.Date - een waarde van Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Haalt een instantie op van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse voor dit object.

--------------------

Alleen lezen ondersteund voor XML-indeling.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Retourneert [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) voor dit object met `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) waarden binnen de opgegeven start- en einddatums.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | De startdatum voor de tijdgephaseerde gegevens. |
| einde | java.util.Date | De einddatum voor de tijdgephaseerde gegevens. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Retourneert een instantie van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse voor dit object met de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) waarden binnen de opgegeven start- en einddatums van het gespecificeerde [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| start | java.util.Date | De startdatum voor de tijdgephaseerde gegevens. |
| einde | java.util.Date | De einddatum voor de tijdgephaseerde gegevens. |
| timephasedType | byte | Het type tijdgephaseerde gegevens ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Haalt een waarde op van Type.

**Returns:**
int - een waarde van Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Haalt een waarde op van Uid.

**Returns:**
int - een waarde van Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Haalt een waarde op van WindowsUserAccount.

**Returns:**
java.lang.String - een waarde van WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Haalt een waarde op van Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Haalt een waarde op van WorkVariance.

**Returns:**
double - een waarde van WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Haalt een waarde op van Workgroup.

**Returns:**
int - een waarde van Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Gereserveerd voor intern gebruik.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Retourneert een hashcode-waarde voor de instantie van de [Resource](../../com.aspose.tasks/resource) klasse.

**Returns:**
int - retourneert een hashcode-waarde voor dit object.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Haalt een waarde op die aangeeft of IsBudget is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Haalt een waarde op die aangeeft of IsCostResource is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Haalt een waarde op die aangeeft of IsEnterprise is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Haalt een waarde op die aangeeft of IsGeneric is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Haalt een waarde op die aangeeft of IsNull is ingesteld of niet.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Haalt de vlag op die aangeeft of de resource een rootresource is. Een rootresource is een speciale resource die bedoeld is om de interne werking van de formaten van MS Project te ondersteunen en niet bedoeld is om rechtstreeks vanuit de code van de gebruiker te worden gebruikt.

**Returns:**
boolean - de vlag die aangeeft of de resource een rootresource is.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Haalt een waarde op die aangeeft of IsTeamAssignmentPool is ingesteld of niet.

**Returns:**
boolean - een waarde die aangeeft of IsTeamAssignmentPool is ingesteld of niet.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | de opgegeven eigenschapssleutel. [Rsc](../../com.aspose.tasks/rsc) voor het verkrijgen van de eigenschapssleutel. |
| val | java.util.Date | de waarde. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Stelt een waarde in voor ACWP.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Stelt een waarde in voor AccrueAt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Stelt een waarde in voor ActiveDirectoryGuid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Stelt een waarde in voor ActualCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van ActualCost. |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Stelt een waarde in voor AvailableFrom.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Stelt een waarde in voor AvailableTo.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van AvailableTo. |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Stelt een waarde in die aangeeft of IsBudget is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of IsBudget is ingesteld of niet. |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Stelt een waarde in voor Calendar.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | een waarde van Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Stelt een waarde in die aangeeft of CanLevel is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of CanLevel is ingesteld of niet. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Stelt een waarde in voor Code.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Stelt een waarde in voor Cost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Stelt een waarde in voor CostCenter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Stelt een waarde in voor CostPerUse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Stelt een waarde in die aangeeft of IsCostResource is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of IsCostResource is ingesteld of niet. |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Stelt een waarde in voor EMailAddress.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Stelt een waarde in die aangeeft of IsEnterprise is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of IsEnterprise is ingesteld of niet. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Stelt een waarde in voor Finish.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Stelt een waarde in die aangeeft of IsGeneric is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of IsGeneric is ingesteld of niet. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Stelt een waarde in voor Group.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Stelt een waarde in voor Guid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Stelt de titel of verklarende tekst van een hyperlink die aan een resource is gekoppeld in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de titel of de verklarende tekst van een hyperlink die aan een resource is gekoppeld. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Stelt het adres in voor een hyperlink die aan een resource is gekoppeld.

--------------------

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | het adres voor een hyperlink die aan een resource is gekoppeld. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Stelt de specifieke locatie in een document in voor een hyperlink die aan een resource is gekoppeld.

--------------------

Het volledige adres (Hyperlink Href in Microsoft Project) van de hyperlink is een samenvoeging van HyperlinkAddress en HyperlinkSubAddress.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de specifieke locatie in een document in een hyperlink die aan een resource is gekoppeld. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Stelt een waarde in voor Id.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Stelt een waarde in die aangeeft of Inactive is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of Inactive is ingesteld of niet. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Stelt een waarde in voor Initials.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Stelt een waarde in voor MaterialLabel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Stelt een waarde in voor MaxUnits.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Stelt een waarde in voor Name.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Stelt een waarde in voor NotesRTF.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Stelt een waarde in voor NotesText.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Stelt een waarde in die aangeeft of IsNull is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of IsNull is ingesteld of niet. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Stelt een waarde in die aangeeft of Overallocated is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | een waarde die aangeeft of Overallocated is ingesteld of niet. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Stelt een waarde in voor OvertimeCost.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Stelt een waarde in voor OvertimeRate.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Stelt een waarde in voor OvertimeRateFormat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van OvertimeRateFormat. |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Stelt een waarde in voor Phonetics.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van Phonetics. |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Stelt een waarde in voor SV.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Stelt een waarde in voor StandardRate.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.math.BigDecimal | een waarde van StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Stelt een waarde in voor StandardRateFormat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Stelt een waarde in voor Start.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date | een waarde van Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Stelt een waarde in die aangeeft of IsTeamAssignmentPool is ingesteld of niet.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of IsTeamAssignmentPool is ingesteld of niet. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Stelt een instantie van [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse in voor dit object.

--------------------

Alleen lezen ondersteund voor XML-indeling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | een instantie van de [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) klasse voor dit object. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Stelt een waarde van Type in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Stelt een waarde van Uid in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Stelt een waarde van WindowsUserAccount in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | een waarde van WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Stelt een waarde van Work in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | een waarde van Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Stelt een waarde van WorkVariance in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | double | een waarde van WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Stelt een waarde van Workgroup in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | een waarde van Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Retourneert een korte tekenreeksrepresentatie van de instantie van de [Resource](../../com.aspose.tasks/resource) klasse. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

**Returns:**
java.lang.String - korte tekenreeks die het resource‑object weergeeft.

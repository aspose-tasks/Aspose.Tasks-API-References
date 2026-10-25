---
title: "Ressource"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Ressource in einem Projekt dar."
type: docs
weight: 248
url: /de/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Stellt eine Ressource in einem Projekt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [canLevel()](#canLevel--) | Gibt einen Wert zurück, der angibt, ob CanLevel gesetzt ist oder nicht. |
| [delete()](#delete--) | Löscht eine Ressource und deren Zuordnungen aus dem Projekt. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einer angegebenen Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse entspricht. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getACWP()](#getACWP--) | Gibt einen Wert von ACWP zurück. |
| [getAccrueAt()](#getAccrueAt--) | Gibt einen Wert von AccrueAt zurück. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Gibt einen Wert von ActiveDirectoryGuid zurück. |
| [getActualCost()](#getActualCost--) | Gibt einen Wert von ActualCost zurück. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Gibt einen Wert von ActualOvertimeCost zurück. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Gibt einen Wert von ActualOvertimeWork zurück. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Gibt einen Wert von ActualOvertimeWorkProtected zurück. |
| [getActualWork()](#getActualWork--) | Gibt einen Wert von ActualWork zurück. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Gibt einen Wert von ActualWorkProtected zurück. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Gibt einen Wert von AssignmentOwner zurück. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Gibt einen Wert von AssignmentOwnerGuid zurück. |
| [getAssignments()](#getAssignments--) | Gibt eine Sammlung von Ressourcenzuweisungen für dieses Objekt zurück. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Gibt die Instanz der [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection)-Klasse zurück. |
| [getAvailableFrom()](#getAvailableFrom--) | Gibt einen Wert von AvailableFrom zurück. |
| [getAvailableTo()](#getAvailableTo--) | Gibt einen Wert von AvailableTo zurück. |
| [getBCWP()](#getBCWP--) | Gibt einen Wert von BCWP zurück. |
| [getBCWS()](#getBCWS--) | Gibt einen Wert von BCWS zurück. |
| [getBaselines()](#getBaselines--) | Gibt eine BaselineCollection-Instanz für dieses Objekt zurück. |
| [getBookingType()](#getBookingType--) | Gibt einen Wert von BookingType zurück. |
| [getBudgetCost()](#getBudgetCost--) | Gibt einen Wert von BudgetCost zurück. |
| [getBudgetWork()](#getBudgetWork--) | Gibt einen Wert von BudgetWork zurück. |
| [getCV()](#getCV--) | Ruft den Wert von CV ab. |
| [getCalendar()](#getCalendar--) | Ruft den Wert von Calendar ab. |
| [getCode()](#getCode--) | Ruft den Wert von Code ab. |
| [getCost()](#getCost--) | Ruft den Wert von Cost ab. |
| [getCostCenter()](#getCostCenter--) | Ruft den Wert von CostCenter ab. |
| [getCostPerUse()](#getCostPerUse--) | Ruft den Wert von CostPerUse ab. |
| [getCostVariance()](#getCostVariance--) | Ruft den Wert von CostVariance ab. |
| [getCreated()](#getCreated--) | Ruft den Wert von Created ab. |
| [getEMailAddress()](#getEMailAddress--) | Ruft den Wert von EMailAddress ab. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Ruft die Werte eines erweiterten Attributs ab. |
| [getFinish()](#getFinish--) | Ruft den Wert von Finish ab. |
| [getGroup()](#getGroup--) | Ruft den Wert von Group ab. |
| [getGuid()](#getGuid--) | Ruft den Wert von Guid ab. |
| [getHyperlink()](#getHyperlink--) | Ruft den Titel oder erläuternden Text eines mit einer Ressource verknüpften Hyperlinks ab. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Ruft die Adresse eines mit einer Ressource verknüpften Hyperlinks ab. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Ruft den spezifischen Ort in einem Dokument eines mit einer Ressource verknüpften Hyperlinks ab. |
| [getId()](#getId--) | Ruft den Wert von Id ab. |
| [getInactive()](#getInactive--) | Ruft einen Wert ab, der angibt, ob Inactive gesetzt ist oder nicht. |
| [getInitials()](#getInitials--) | Ruft den Wert von Initials ab. |
| [getItems()](#getItems--) | Ruft untergeordnete Ressourcen ab. |
| [getMaterialLabel()](#getMaterialLabel--) | Ruft den Wert von MaterialLabel ab. |
| [getMaxUnits()](#getMaxUnits--) | Ruft den Wert von MaxUnits ab. |
| [getName()](#getName--) | Ruft den Wert von Name ab. |
| [getNotesRTF()](#getNotesRTF--) | Ruft den Wert von NotesRTF ab. |
| [getNotesText()](#getNotesText--) | Ruft den Wert von NotesText ab. |
| [getOutlineCode()](#getOutlineCode--) | Liefert ein OutlineCodeCollection-Objekt. |
| [getOverallocated()](#getOverallocated--) | Liefert einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |
| [getOvertimeCost()](#getOvertimeCost--) | Liefert einen Wert von OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Liefert einen Wert von OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Liefert einen Wert von OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Liefert einen Wert von OvertimeWork. |
| [getParentProject()](#getParentProject--) | Liefert das übergeordnete Projekt für diesen Container. |
| [getPeakUnits()](#getPeakUnits--) | Liefert einen Wert von PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Liefert einen Wert von PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Liefert einen Wert von Phonetics. |
| [getRates()](#getRates--) | Liefert die Instanz der [RateCollection](../../com.aspose.tasks/ratecollection)-Klasse für dieses Objekt. |
| [getRegularWork()](#getRegularWork--) | Liefert einen Wert von RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Liefert einen Wert von RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Liefert einen Wert von RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Liefert einen Wert von RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Liefert einen Wert von RemainingWork. |
| [getSV()](#getSV--) | Liefert einen Wert von SV. |
| [getStandardRate()](#getStandardRate--) | Liefert einen Wert von StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Liefert einen Wert von StandardRateFormat. |
| [getStart()](#getStart--) | Liefert einen Wert von Start. |
| [getTimephasedData()](#getTimephasedData--) | Liefert eine Instanz der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Klasse für dieses Objekt. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Gibt [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt zurück, mit `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) Werte innerhalb der angegebenen Start- und Enddaten. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Gibt eine Instanz der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Klasse für dieses Objekt zurück, mit den `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) Werte innerhalb der angegebenen Start- und Enddaten des angegebenen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Liefert einen Wert von Type. |
| [getUid()](#getUid--) | Liefert einen Wert von Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Ermittelt einen Wert von WindowsUserAccount. |
| [getWork()](#getWork--) | Ermittelt einen Wert von Work. |
| [getWorkVariance()](#getWorkVariance--) | Ermittelt einen Wert von WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Ermittelt einen Wert von Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse zurück. |
| [isBudget()](#isBudget--) | Ermittelt einen Wert, der angibt, ob IsBudget gesetzt ist oder nicht. |
| [isCostResource()](#isCostResource--) | Ermittelt einen Wert, der angibt, ob IsCostResource gesetzt ist oder nicht. |
| [isEnterprise()](#isEnterprise--) | Ermittelt einen Wert, der angibt, ob IsEnterprise gesetzt ist oder nicht. |
| [isGeneric()](#isGeneric--) | Ermittelt einen Wert, der angibt, ob IsGeneric gesetzt ist oder nicht. |
| [isNull()](#isNull--) | Ermittelt einen Wert, der angibt, ob IsNull gesetzt ist oder nicht. |
| [isRoot()](#isRoot--) | Ermittelt das Flag, das angibt, ob resource eine Root‑Ressource ist. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Ermittelt einen Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [setACWP(double value)](#setACWP-double-) | Setzt einen Wert von ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Setzt einen Wert von AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Setzt einen Wert von ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Setzt einen Wert von ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert von ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Setzt einen Wert von AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Setzt einen Wert von AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Setzt einen Wert von AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Setzt einen Wert von AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Setzt einen Wert für BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Setzt einen Wert für BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Setzt einen Wert für BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob IsBudget gesetzt ist oder nicht. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Setzt einen Wert für BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Setzt einen Wert für BudgetWork. |
| [setCV(double value)](#setCV-double-) | Setzt einen Wert für CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Setzt einen Wert für Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob CanLevel gesetzt ist oder nicht. |
| [setCode(String value)](#setCode-java.lang.String-) | Setzt einen Wert für Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Setzt einen Wert für Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Setzt einen Wert für CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Setzt einen Wert für CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob IsCostResource gesetzt ist oder nicht. |
| [setCostVariance(double value)](#setCostVariance-double-) | Setzt einen Wert für CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Setzt einen Wert für Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Setzt einen Wert für EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob IsEnterprise gesetzt ist oder nicht. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Setzt einen Wert für Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob IsGeneric gesetzt ist oder nicht. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Setzt einen Wert für Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Setzt einen Wert für Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Setzt den Titel oder erklärenden Text eines mit einer Ressource verknüpften Hyperlinks. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Setzt die Adresse für einen mit einer Ressource verknüpften Hyperlink. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Setzt den spezifischen Ort in einem Dokument in einem mit einer Ressource verknüpften Hyperlink. |
| [setId(int value)](#setId-int-) | Setzt einen Wert für Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob Inactive gesetzt ist oder nicht. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Setzt einen Wert für Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Setzt einen Wert für MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Setzt einen Wert für MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Setzt einen Wert für Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Setzt einen Wert für NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Setzt einen Wert für NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob IsNull gesetzt ist oder nicht. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Setzt einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert für OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Setzt einen Wert für OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Setzt einen Wert für OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert für OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Setzt einen Wert für PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Setzt einen Wert für PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Setzt einen Wert für Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Setzt einen Wert für RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert für RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RemainingWork. |
| [setSV(double value)](#setSV-double-) | Setzt einen Wert für SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Setzt einen Wert für StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Setzt einen Wert für StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Setzt einen Wert für Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Setzt einen Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Setzt eine Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt. |
| [setType(int value)](#setType-int-) | Setzt einen Wert für Type. |
| [setUid(int value)](#setUid-int-) | Setzt einen Wert für Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Setzt einen Wert für WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Setzt einen Wert für Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Setzt einen Wert für WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Setzt einen Wert für Workgroup. |
| [toString()](#toString--) | Gibt die kurze Zeichenkettenrepräsentation der Instanz der Klasse [Resource](../../com.aspose.tasks/resource) zurück. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | der angegebene Eigenschaftsschlüssel. [Rsc](../../com.aspose.tasks/rsc) zum Abrufen des Eigenschaftsschlüssels. |

**Returns:**
T - der Wert, dem die Eigenschaft in diesem Container zugeordnet ist.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | der angegebene Eigenschaftsschlüssel. [Rsc](../../com.aspose.tasks/rsc) zum Abrufen des Eigenschaftsschlüssels. |
| val | T | der Wert. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Gibt einen Wert zurück, der angibt, ob CanLevel gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Löscht eine Ressource und deren Zuordnungen aus dem Projekt.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einer angegebenen Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse entspricht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | Die angegebene Instanz der Klasse [Resource](../../com.aspose.tasks/resource), die mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True**, wenn die angegebene Instanz der Klasse [Resource](../../com.aspose.tasks/resource) denselben Uid-Wert wie diese Instanz hat; andernfalls **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt, das mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True**, wenn das angegebene Objekt ein Resource ist, das denselben Uid-Wert wie diese Instanz hat; andernfalls **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Gibt einen Wert von ACWP zurück.

**Returns:**
double - ein Wert von ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Gibt einen Wert von AccrueAt zurück.

**Returns:**
int - ein Wert von AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Gibt einen Wert von ActiveDirectoryGuid zurück.

**Returns:**
java.lang.String - ein Wert von ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Gibt einen Wert von ActualCost zurück.

**Returns:**
java.math.BigDecimal - ein Wert von ActualCost.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Gibt einen Wert von ActualOvertimeCost zurück.

**Returns:**
java.math.BigDecimal - ein Wert von ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Gibt einen Wert von ActualOvertimeWork zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Gibt einen Wert von ActualOvertimeWorkProtected zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Gibt einen Wert von ActualWork zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Gibt einen Wert von ActualWorkProtected zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Gibt einen Wert von AssignmentOwner zurück.

**Returns:**
java.lang.String - ein Wert von AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Gibt einen Wert von AssignmentOwnerGuid zurück.

**Returns:**
java.lang.String - ein Wert von AssignmentOwnerGuid.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Gibt eine Sammlung von Ressourcenzuweisungen für dieses Objekt zurück.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Liefert die Instanz der [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection)-Klasse. Die Sammlung von Zeiträumen, in denen eine Ressource verfügbar ist.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Gibt einen Wert von AvailableFrom zurück.

**Returns:**
java.util.Date - ein Wert von AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Gibt einen Wert von AvailableTo zurück.

**Returns:**
java.util.Date - ein Wert von AvailableTo.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Gibt einen Wert von BCWP zurück.

**Returns:**
double - ein Wert von BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Gibt einen Wert von BCWS zurück.

**Returns:**
double - ein Wert von BCWS.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Liefert eine BaselineCollection-Instanz für dieses Objekt. Die Basislinienwerte für eine Ressource.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Gibt einen Wert von BookingType zurück.

**Returns:**
int - ein Wert von BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Gibt einen Wert von BudgetCost zurück.

**Returns:**
java.math.BigDecimal - ein Wert von BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Gibt einen Wert von BudgetWork zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Ruft den Wert von CV ab.

**Returns:**
double - ein Wert von CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Ruft den Wert von Calendar ab.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Ruft den Wert von Code ab.

**Returns:**
java.lang.String - ein Wert von Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ruft den Wert von Cost ab.

**Returns:**
java.math.BigDecimal - ein Wert von Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Ruft den Wert von CostCenter ab.

**Returns:**
java.lang.String - ein Wert von CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Ruft den Wert von CostPerUse ab.

**Returns:**
java.math.BigDecimal - ein Wert von CostPerUse.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Ruft den Wert von CostVariance ab.

**Returns:**
double - ein Wert von CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Ruft den Wert von Created ab.

**Returns:**
java.util.Date - ein Wert von Created.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Ruft den Wert von EMailAddress ab.

**Returns:**
java.lang.String - ein Wert von EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Ruft die Werte eines erweiterten Attributs ab.

--------------------

Zwei Datenstücke sind erforderlich – ein Verweis zurück auf die erweiterte Attributtabelle, die entweder über die eindeutige ID oder die Feld-ID angegeben wird, und der Wert, der entweder direkt angegeben wird oder ein Verweis zurück auf die Wertliste ist.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ruft den Wert von Finish ab.

**Returns:**
java.util.Date - ein Wert von Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Ruft den Wert von Group ab.

**Returns:**
java.lang.String - ein Wert von Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Ruft den Wert von Guid ab.

**Returns:**
java.lang.String - ein Wert von Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Ruft den Titel oder erläuternden Text eines mit einer Ressource verknüpften Hyperlinks ab.

**Returns:**
java.lang.String - der Titel oder erläuternde Text eines mit einer Ressource verknüpften Hyperlinks.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Ruft die Adresse eines mit einer Ressource verknüpften Hyperlinks ab.

--------------------

Die vollständige Adresse (Hyperlink Href in Microsoft Project) des Hyperlinks ist eine Verkettung von HyperlinkAddress und HyperlinkSubAddress.

**Returns:**
java.lang.String - die Adresse eines mit einer Ressource verknüpften Hyperlinks.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Ruft den spezifischen Ort in einem Dokument eines mit einer Ressource verknüpften Hyperlinks ab.

--------------------

Die vollständige Adresse (Hyperlink Href in Microsoft Project) des Hyperlinks ist eine Verkettung von HyperlinkAddress und HyperlinkSubAddress.

**Returns:**
java.lang.String - der spezifische Ort in einem Dokument in einem mit einer Ressource verknüpften Hyperlink.
### getId() {#getId--}
```
public final int getId()
```


Ruft den Wert von Id ab.

**Returns:**
int - ein Wert von Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Ruft einen Wert ab, der angibt, ob Inactive gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Ruft den Wert von Initials ab.

**Returns:**
java.lang.String - ein Wert von Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Ruft untergeordnete Ressourcen ab.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - untergeordnete Ressourcen.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Ruft den Wert von MaterialLabel ab.

**Returns:**
java.lang.String - ein Wert von MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Ruft den Wert von MaxUnits ab.

**Returns:**
double - ein Wert von MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Ruft den Wert von Name ab.

**Returns:**
java.lang.String - ein Wert von Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Ruft den Wert von NotesRTF ab.

**Returns:**
java.lang.String - ein Wert von NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Ruft den Wert von NotesText ab.

**Returns:**
java.lang.String - ein Wert von NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Liefert ein OutlineCodeCollection-Objekt. Der Wert eines Gliederungscodes.

--------------------

Zwei Datenstücke sind erforderlich - ein Zeiger auf die Gliederungscode‑Tabelle, die durch die FieldID angegeben ist, und der Wert, der entweder durch die ValueID oder den ValueGUID‑Zeiger auf die Wertliste angegeben wird.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Liefert einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Liefert einen Wert von OvertimeCost.

**Returns:**
java.math.BigDecimal - ein Wert von OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Liefert einen Wert von OvertimeRate.

**Returns:**
java.math.BigDecimal - ein Wert von OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Liefert einen Wert von OvertimeRateFormat.

**Returns:**
int - ein Wert von OvertimeRateFormat.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Liefert einen Wert von OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Liefert das übergeordnete Projekt für diesen Container.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Liefert einen Wert von PeakUnits.

**Returns:**
double - ein Wert von PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Liefert einen Wert von PercentWorkComplete.

**Returns:**
int - ein Wert von PercentWorkComplete.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Liefert einen Wert von Phonetics.

**Returns:**
java.lang.String - ein Wert von Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Liefert die Instanz der [RateCollection](../../com.aspose.tasks/ratecollection)-Klasse für dieses Objekt. Die Sammlung von Zeiträumen und Raten, die jeweils zugeordnet sind.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Liefert einen Wert von RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Liefert einen Wert von RemainingCost.

**Returns:**
java.math.BigDecimal - ein Wert von RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Liefert einen Wert von RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - ein Wert von RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Liefert einen Wert von RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Liefert einen Wert von RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


Liefert einen Wert von SV.

**Returns:**
double - ein Wert von SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Liefert einen Wert von StandardRate.

**Returns:**
java.math.BigDecimal - ein Wert von StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Liefert einen Wert von StandardRateFormat.

**Returns:**
int - ein Wert von StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Liefert einen Wert von Start.

**Returns:**
java.util.Date - ein Wert von Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Liefert eine Instanz der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Klasse für dieses Objekt.

--------------------

Lesen wird nur für das XML-Format unterstützt.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Gibt [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt zurück, mit `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) Werte innerhalb der angegebenen Start- und Enddaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Das Startdatum für die zeitphasierten Daten. |
| Ende | java.util.Date | Das Enddatum für die zeitphasierten Daten. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Gibt eine Instanz der [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)-Klasse für dieses Objekt zurück, mit den `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) Werte innerhalb der angegebenen Start- und Enddaten des angegebenen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Das Startdatum für die zeitphasierten Daten. |
| Ende | java.util.Date | Das Enddatum für die zeitphasierten Daten. |
| timephasedType | byte | Der Typ der zeitphasierten Daten ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Liefert einen Wert von Type.

**Returns:**
int - ein Wert des Typs.
### getUid() {#getUid--}
```
public final int getUid()
```


Liefert einen Wert von Uid.

**Returns:**
int - ein Wert von Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Ermittelt einen Wert von WindowsUserAccount.

**Returns:**
java.lang.String - ein Wert von WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ermittelt einen Wert von Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Ermittelt einen Wert von WorkVariance.

**Returns:**
double - ein Wert von WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Ermittelt einen Wert von Workgroup.

**Returns:**
int - ein Wert von Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Für den internen Gebrauch reserviert.

**Returns:**
boolean - \\{@inheritDoc\\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der [Resource](../../com.aspose.tasks/resource)-Klasse zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Ermittelt einen Wert, der angibt, ob IsBudget gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Ermittelt einen Wert, der angibt, ob IsCostResource gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Ermittelt einen Wert, der angibt, ob IsEnterprise gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Ermittelt einen Wert, der angibt, ob IsGeneric gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Ermittelt einen Wert, der angibt, ob IsNull gesetzt ist oder nicht.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Gibt das Flag zurück, das angibt, ob die Ressource eine Root resource ist. Root resource ist eine spezielle Ressource, die dazu dient, die internen Strukturen der MS Project‑Formate zu unterstützen und nicht dazu gedacht ist, direkt aus dem Code des Benutzers verwendet zu werden.

**Returns:**
boolean - das Flag, das angibt, ob die Ressource eine Root resource ist.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Ermittelt einen Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | der angegebene Eigenschaftsschlüssel. [Rsc](../../com.aspose.tasks/rsc) zum Abrufen des Eigenschaftsschlüssels. |
| val | java.util.Date | der Wert. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Setzt einen Wert von ACWP.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Setzt einen Wert von AccrueAt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Setzt einen Wert von ActiveDirectoryGuid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Setzt einen Wert von ActualCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von ActualCost. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Setzt einen Wert von ActualOvertimeCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Setzt einen Wert von ActualOvertimeWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Setzt einen Wert von ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von ActualOvertimeWorkProtected. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Setzt einen Wert von ActualWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Setzt einen Wert von ActualWorkProtected.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Setzt einen Wert von AssignmentOwner.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Setzt einen Wert von AssignmentOwnerGuid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von AssignmentOwnerGuid. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Setzt einen Wert von AvailableFrom.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Setzt einen Wert von AvailableTo.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von AvailableTo. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Setzt einen Wert für BCWP.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Setzt einen Wert für BCWS.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Setzt einen Wert für BookingType.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von BookingType. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Setzt einen Wert, der angibt, ob IsBudget gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob IsBudget gesetzt ist oder nicht. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Setzt einen Wert für BudgetCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Setzt einen Wert für BudgetWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Setzt einen Wert für CV.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Setzt einen Wert für Calendar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | ein Wert von Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Setzt einen Wert, der angibt, ob CanLevel gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob CanLevel gesetzt ist oder nicht. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Setzt einen Wert für Code.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Setzt einen Wert für Cost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Setzt einen Wert für CostCenter.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Setzt einen Wert für CostPerUse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Setzt einen Wert, der angibt, ob IsCostResource gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob IsCostResource gesetzt ist oder nicht. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Setzt einen Wert für CostVariance.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Setzt einen Wert für Created.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Created. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Setzt einen Wert für EMailAddress.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Setzt einen Wert, der angibt, ob IsEnterprise gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob IsEnterprise gesetzt ist oder nicht. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Setzt einen Wert für Finish.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Setzt einen Wert, der angibt, ob IsGeneric gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob IsGeneric gesetzt ist oder nicht. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Setzt einen Wert für Group.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Setzt einen Wert für Guid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Setzt den Titel oder erklärenden Text eines mit einer Ressource verknüpften Hyperlinks.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der Titel oder erläuternde Text eines Hyperlinks, der mit einer Ressource verknüpft ist. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Setzt die Adresse für einen mit einer Ressource verknüpften Hyperlink.

--------------------

Die vollständige Adresse (Hyperlink Href in Microsoft Project) des Hyperlinks ist eine Verkettung von HyperlinkAddress und HyperlinkSubAddress.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Adresse eines Hyperlinks, der mit einer Ressource verknüpft ist. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Setzt den spezifischen Ort in einem Dokument in einem mit einer Ressource verknüpften Hyperlink.

--------------------

Die vollständige Adresse (Hyperlink Href in Microsoft Project) des Hyperlinks ist eine Verkettung von HyperlinkAddress und HyperlinkSubAddress.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der spezifische Ort in einem Dokument in einem Hyperlink, der mit einer Ressource verknüpft ist. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Setzt einen Wert für Id.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Setzt einen Wert, der angibt, ob Inactive gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob Inactive gesetzt ist oder nicht. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Setzt einen Wert für Initials.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Initialen. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Setzt einen Wert für MaterialLabel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Setzt einen Wert für MaxUnits.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Setzt einen Wert für Name.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Setzt einen Wert für NotesRTF.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Setzt einen Wert für NotesText.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Setzt einen Wert, der angibt, ob IsNull gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob IsNull gesetzt ist oder nicht. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Setzt einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | ein Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Setzt einen Wert für OvertimeCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Setzt einen Wert für OvertimeRate.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Setzt einen Wert für OvertimeRateFormat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von OvertimeRateFormat. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Setzt einen Wert für OvertimeWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Setzt einen Wert für PeakUnits.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Setzt einen Wert für PercentWorkComplete.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von PercentWorkComplete. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Setzt einen Wert für Phonetics.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Phonetics. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Setzt einen Wert für RegularWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Setzt einen Wert für RemainingCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Setzt einen Wert für RemainingOvertimeCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Setzt einen Wert für RemainingOvertimeWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Setzt einen Wert für RemainingWork.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von RemainingWork. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Setzt einen Wert für SV.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Setzt einen Wert für StandardRate.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Setzt einen Wert für StandardRateFormat.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Setzt einen Wert für Start.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Setzt einen Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob IsTeamAssignmentPool gesetzt ist oder nicht. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Setzt eine Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt.

--------------------

Lesen wird nur für das XML-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | eine Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) für dieses Objekt. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Setzt einen Wert für Type.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Setzt einen Wert für Uid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Setzt einen Wert für WindowsUserAccount.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Setzt einen Wert für Work.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Setzt einen Wert für WorkVariance.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Setzt einen Wert für Workgroup.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Gibt die kurze Zeichenkettenrepräsentation der Instanz der Klasse [Resource](../../com.aspose.tasks/resource) zurück. Die genauen Details der Darstellung sind nicht spezifiziert und können sich ändern.

**Returns:**
java.lang.String – kurze Zeichenkette, die das Ressourcenobjekt darstellt.

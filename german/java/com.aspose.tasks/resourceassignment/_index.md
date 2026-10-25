---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Ressourcenzuweisung in einem Projekt dar."
type: docs
weight: 249
url: /de/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Stellt eine Ressourcenzuweisung in einem Projekt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| [delete()](#delete--) | Löscht die Ressourcenzuweisung aus der Sammlung der Projektzuweisungen. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Gibt einen Wert zurück, der angibt, ob diese Instanz gleich einer angegebenen Instanz der [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Klasse ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Gibt einen Wert zurück, der angibt, ob diese Instanz einem angegebenen Objekt gleich ist. |
| [getACWP()](#getACWP--) | Gibt einen Wert von ACWP zurück. |
| [getActualCost()](#getActualCost--) | Gibt einen Wert von ActualCost zurück. |
| [getActualFinish()](#getActualFinish--) | Gibt einen Wert von ActualFinish zurück. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Gibt einen Wert von ActualOvertimeCost zurück. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Gibt einen Wert von ActualOvertimeWork zurück. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Gibt einen Wert von ActualOvertimeWorkProtected zurück. |
| [getActualStart()](#getActualStart--) | Gibt einen Wert von ActualStart zurück. |
| [getActualWork()](#getActualWork--) | Gibt einen Wert von ActualWork zurück. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Gibt einen Wert von ActualWorkProtected zurück. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Gibt einen Wert von AssignmentOwner zurück. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Gibt einen Wert von AssignmentOwnerGuid zurück. |
| [getBCWP()](#getBCWP--) | Gibt einen Wert von BCWP zurück. |
| [getBCWS()](#getBCWS--) | Gibt einen Wert von BCWS zurück. |
| [getBaselines()](#getBaselines--) | Liefert das AssignmentBaselineCollection-Objekt. |
| [getBookingType()](#getBookingType--) | Gibt einen Wert von BookingType zurück. |
| [getBudgetCost()](#getBudgetCost--) | Gibt einen Wert von BudgetCost zurück. |
| [getBudgetWork()](#getBudgetWork--) | Gibt einen Wert von BudgetWork zurück. |
| [getCV()](#getCV--) | Ruft den Wert von CV ab. |
| [getConfirmed()](#getConfirmed--) | Liefert einen Wert, der angibt, ob Confirmed gesetzt ist oder nicht. |
| [getCost()](#getCost--) | Ruft den Wert von Cost ab. |
| [getCostRateTableType()](#getCostRateTableType--) | Gibt einen Wert von CostRateTableType zurück. |
| [getCostVariance()](#getCostVariance--) | Ruft den Wert von CostVariance ab. |
| [getCreated()](#getCreated--) | Ruft den Wert von Created ab. |
| [getDelay()](#getDelay--) | Gibt einen Wert von Delay zurück. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Liefert eine Instanz der Klasse ExtendedAttributeCollection für dieses Objekt. |
| [getFinish()](#getFinish--) | Ruft den Wert von Finish ab. |
| [getFinishVariance()](#getFinishVariance--) | Gibt einen Wert von FinishVariance zurück. |
| [getFixedMaterial()](#getFixedMaterial--) | Liefert einen Wert, der angibt, ob FixedMaterial gesetzt ist oder nicht. |
| [getGuid()](#getGuid--) | Liefert die eindeutige Kennung für diese Zuweisung. |
| [getHyperlink()](#getHyperlink--) | Gibt einen Wert von Hyperlink zurück. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Gibt einen Wert von HyperlinkAddress zurück. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Gibt einen Wert von HyperlinkSubAddress zurück. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Gibt einen Wert von LevelingDelay zurück. |
| [getLinkedFields()](#getLinkedFields--) | Liefert einen Wert, der angibt, ob LinkedFields gesetzt ist oder nicht. |
| [getMilestone()](#getMilestone--) | Liefert einen Wert, der angibt, ob Milestone gesetzt ist oder nicht. |
| [getNotesRTF()](#getNotesRTF--) | Liefert die Textnotizen im RTF-Format. |
| [getNotesText()](#getNotesText--) | Liefert den Klartext der Notizen, extrahiert aus RTF-Daten. |
| [getOverallocated()](#getOverallocated--) | Liefert einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |
| [getOvertimeCost()](#getOvertimeCost--) | Liefert einen Wert von OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Liefert einen Wert von OvertimeWork. |
| [getParentProject()](#getParentProject--) | Liefert das übergeordnete Projekt für diese Zuweisung. |
| [getPeakUnits()](#getPeakUnits--) | Liefert einen Wert von PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Liefert einen Wert von PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Ruft den Wert von RateScale ab. |
| [getRegularWork()](#getRegularWork--) | Liefert einen Wert von RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Liefert einen Wert von RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Liefert einen Wert von RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Liefert einen Wert von RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Liefert einen Wert von RemainingWork. |
| [getResource()](#getResource--) | Die einer Aufgabe zugewiesene Ressource. |
| [getResponsePending()](#getResponsePending--) | Ruft einen Wert ab, der angibt, ob ResponsePending gesetzt ist oder nicht. |
| [getResume()](#getResume--) | Ruft den Wert von Resume ab. |
| [getSV()](#getSV--) | Liefert einen Wert von SV. |
| [getStart()](#getStart--) | Liefert einen Wert von Start. |
| [getStartVariance()](#getStartVariance--) | Ruft den Wert von StartVariance ab. |
| [getStop()](#getStop--) | Ruft den Wert von Stop ab. |
| [getSummary()](#getSummary--) | Ruft einen Wert ab, der angibt, ob Summary gesetzt ist oder nicht. |
| [getTask()](#getTask--) | Die Aufgabe, der eine Ressource zugewiesen ist. |
| [getTimephasedData()](#getTimephasedData--) | Ruft die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ab, die Elemente von `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) enthält. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Gibt ein Objekt der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) zurück, das Instanzen von `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) innerhalb des angegebenen Start- und Enddatums von [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) enthält. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Gibt die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) zurück, die Instanzen von `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) innerhalb der angegebenen Start- und Enddaten des angegebenen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) enthält. |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Ruft die Menge der zeitphasierten Arbeit für das angegebene Datumszeitintervall ab. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Ruft die Menge der zeitphasierten Arbeit für das angegebene Datumszeitintervall ab. |
| [getUid()](#getUid--) | Liefert einen Wert von Uid. |
| [getUnits()](#getUnits--) | Ruft den Wert von Units ab. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Ruft einen Wert ab, der angibt, ob UpdateNeeded gesetzt ist oder nicht. |
| [getVAC()](#getVAC--) | Ruft den Wert von VAC ab. |
| [getWork()](#getWork--) | Ermittelt einen Wert von Work. |
| [getWorkContour()](#getWorkContour--) | Ruft den Wert von WorkContour ab. |
| [getWorkVariance()](#getWorkVariance--) | Ermittelt einen Wert von WorkVariance. |
| [hasChildren()](#hasChildren--) | Ruft einen Wert ab, der anzeigt, dass diese Ressourcen-Zuweisung untergeordnete Elemente hat. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Ruft einen Wert ab, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht. |
| [hashCode()](#hashCode--) | Gibt einen Hashcode-Wert für die Instanz der Klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment) zurück. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Erzeugt eine Liste von zeitphasierten Daten. |
| [setACWP(double value)](#setACWP-double-) | Setzt einen Wert von ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Setzt einen Wert von ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Setzt einen Wert von ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert von ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Setzt einen Wert von ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Setzt einen Wert von ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Setzt einen Wert von AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Setzt einen Wert von AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Setzt einen Wert für BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Setzt einen Wert für BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Setzt einen Wert für BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Setzt einen Wert für BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Setzt einen Wert für BudgetWork. |
| [setCV(double value)](#setCV-double-) | Setzt einen Wert für CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Setzt einen Wert, der angibt, ob Confirmed gesetzt ist oder nicht. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Setzt einen Wert für Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Setzt einen Wert von CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Setzt einen Wert für CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Setzt einen Wert für Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Setzt einen Wert von Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Setzt eine Instanz der Klasse ExtendedAttributeCollection für dieses Objekt. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Setzt einen Wert für Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Setzt einen Wert von FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Legt einen Wert fest, der angibt, ob FixedMaterial gesetzt ist oder nicht. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Legt einen Wert fest, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Legt die eindeutige Kennung für diese Zuordnung fest. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Legt einen Wert für Hyperlink fest. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Legt einen Wert für HyperlinkAddress fest. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Legt einen Wert für HyperlinkSubAddress fest. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Legt einen Wert für LevelingDelay fest. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Legt einen Wert fest, der angibt, ob LinkedFields gesetzt ist oder nicht. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Legt Einheiten für die Zuordnung einer Materialressource mit variablem Materialverbrauch fest. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Legt einen Wert fest, der angibt, ob Milestone gesetzt ist oder nicht. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Legt die Textnotizen im RTF-Format fest. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Legt den Klartext der Notizen fest, der aus RTF-Daten extrahiert wurde. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Setzt einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert für OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert für OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Setzt einen Wert für PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Setzt einen Wert für PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Legt einen Wert für RateScale fest. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Setzt einen Wert für RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Setzt einen Wert für RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Setzt einen Wert für RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | Die einer Aufgabe zugewiesene Ressource. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Legt einen Wert fest, der angibt, ob ResponsePending gesetzt ist oder nicht. |
| [setResume(Date value)](#setResume-java.util.Date-) | Legt einen Wert für Resume fest. |
| [setSV(double value)](#setSV-double-) | Setzt einen Wert für SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Setzt einen Wert für Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Legt einen Wert für StartVariance fest. |
| [setStop(Date value)](#setStop-java.util.Date-) | Legt einen Wert für Stop fest. |
| [setSummary(boolean value)](#setSummary-boolean-) | Legt einen Wert fest, der angibt, ob Summary gesetzt ist oder nicht. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | Die Aufgabe, der eine Ressource zugewiesen ist. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Legt die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) fest, die Elemente von `TimephasedData` ([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) enthält. |
| [setUid(int value)](#setUid-int-) | Setzt einen Wert für Uid. |
| [setUnits(double value)](#setUnits-double-) | Legt einen Wert für Units fest. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Legt einen Wert fest, der angibt, ob UpdateNeeded gesetzt ist oder nicht. |
| [setVAC(double value)](#setVAC-double-) | Legt einen Wert für VAC fest. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Setzt einen Wert für Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Legt einen Wert für WorkContour fest. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Setzt einen Wert für WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Teilt die Aufgabe in zwei Teile. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Erzeugt eine Liste von zeitlich gestaffelten Daten basierend auf der Aufgabendauer und dem geplanten Startdatum. |
| [toString()](#toString--) | Gibt die kurze Zeichenkettenrepräsentation der Instanz der [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Klasse zurück. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | Der angegebene Eigenschaftsschlüssel. [Asn](../../com.aspose.tasks/asn) zum Abrufen des Eigenschaftsschlüssels. |

**Returns:**
T - der Wert, dem die Eigenschaft in diesem Container zugeordnet ist.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | Der angegebene Eigenschaftsschlüssel. [Asn](../../com.aspose.tasks/asn) zum Abrufen des Eigenschaftsschlüssels. |
| val | T | der Wert. |

### delete() {#delete--}
```
public final void delete()
```


Löscht die Ressourcenzuweisung aus der Sammlung der Projektzuweisungen.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Gibt einen Wert zurück, der angibt, ob diese Instanz gleich einer angegebenen Instanz der [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Klasse ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Die angegebene Instanz der [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Klasse, die mit dieser Instanz verglichen wird. |

**Returns:**
boolean - **True**, wenn die angegebene Instanz der [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Klasse denselben UID-Wert wie diese Instanz hat; andernfalls **false**.
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
boolean - **True**, wenn o ein ResourceAssignment ist, das dieselbe Ressource und Aufgabe wie diese Instanz zuweist; andernfalls **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Gibt einen Wert von ACWP zurück.

**Returns:**
double - ein Wert von ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Gibt einen Wert von ActualCost zurück.

**Returns:**
java.math.BigDecimal - ein Wert von ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Gibt einen Wert von ActualFinish zurück.

**Returns:**
java.util.Date - ein Wert von ActualFinish.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Gibt einen Wert von ActualStart zurück.

**Returns:**
java.util.Date - ein Wert von ActualStart.
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
public final AssignmentBaselineCollection getBaselines()
```


Liefert das AssignmentBaselineCollection-Objekt. Die Sammlung von Basislinienwerten, die mit einer Zuordnung verknüpft sind.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Liefert einen Wert, der angibt, ob Confirmed gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob Confirmed gesetzt ist oder nicht.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Ruft den Wert von Cost ab.

**Returns:**
java.math.BigDecimal - ein Wert von Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Gibt einen Wert von CostRateTableType zurück.

**Returns:**
int - ein Wert von CostRateTableType.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Gibt einen Wert von Delay zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Liefert eine Instanz der Klasse ExtendedAttributeCollection für dieses Objekt.

--------------------

Lesen wird nur für das XML-Format unterstützt.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Ruft den Wert von Finish ab.

**Returns:**
java.util.Date - ein Wert von Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Gibt einen Wert von FinishVariance zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Liefert einen Wert, der angibt, ob FixedMaterial gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob FixedMaterial gesetzt ist oder nicht.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Liefert die eindeutige Kennung für diese Zuweisung.

**Returns:**
java.util.UUID - eindeutiger Bezeichner für diese Zuordnung.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Gibt einen Wert von Hyperlink zurück.

**Returns:**
java.lang.String - ein Wert von Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Gibt einen Wert von HyperlinkAddress zurück.

**Returns:**
java.lang.String - ein Wert von HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Gibt einen Wert von HyperlinkSubAddress zurück.

**Returns:**
java.lang.String - ein Wert von HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Für den internen Gebrauch reserviert.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Gibt einen Wert von LevelingDelay zurück.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Liefert einen Wert, der angibt, ob LinkedFields gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob LinkedFields gesetzt ist oder nicht.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Liefert einen Wert, der angibt, ob Milestone gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob Milestone gesetzt ist oder nicht.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Liefert die Textnotizen im RTF-Format.

--------------------

Nur für MPP-Formate unterstützt.

**Returns:**
java.lang.String - die Textnotizen im RTF-Format.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Liefert den Klartext der Notizen, extrahiert aus RTF-Daten.

**Returns:**
java.lang.String - der reine Text der Notizen, extrahiert aus RTF-Daten.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Liefert einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob Overallocated gesetzt ist oder nicht.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Liefert einen Wert von OvertimeCost.

**Returns:**
java.math.BigDecimal - ein Wert von OvertimeCost.
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


Liefert das übergeordnete Projekt für diese Zuweisung.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Ruft den Wert von RateScale ab.

**Returns:**
int - ein Wert von RateScale.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


Die einer Aufgabe zugewiesene Ressource.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Ruft einen Wert ab, der angibt, ob ResponsePending gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob ResponsePending gesetzt ist oder nicht.
### getResume() {#getResume--}
```
public final Date getResume()
```


Ruft den Wert von Resume ab.

**Returns:**
java.util.Date - ein Wert von Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Liefert einen Wert von SV.

**Returns:**
double - ein Wert von SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Liefert einen Wert von Start.

**Returns:**
java.util.Date - ein Wert von Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Ruft den Wert von StartVariance ab.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Ruft den Wert von Stop ab.

**Returns:**
java.util.Date - ein Wert von Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Ruft einen Wert ab, der angibt, ob Summary gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob Summary gesetzt ist oder nicht.
### getTask() {#getTask--}
```
public final Task getTask()
```


Die Aufgabe, der eine Ressource zugewiesen ist.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Ruft die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) ab, die Elemente von `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) enthält.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Gibt ein Objekt der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) zurück, das Instanzen von `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) innerhalb des angegebenen Start- und Enddatums von [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Das Startdatum für die zeitphasierten Daten. |
| Ende | java.util.Date | Das Enddatum für die zeitphasierten Daten. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Gibt die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) zurück, die Instanzen von `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) innerhalb der angegebenen Start- und Enddaten des angegebenen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Das Startdatum für die zeitphasierten Daten. |
| Ende | java.util.Date | Das Enddatum für die zeitphasierten Daten. |
| timephasedType | byte | Der Typ der zeitphasierten Daten ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Ruft die Menge der zeitphasierten Arbeit für das angegebene Datumszeitintervall ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Start des Datums‑Zeit‑Intervalls. |
| Ende | java.util.Date | Ende des Datums‑Zeit‑Intervalls. |

**Returns:**
double - Menge an zeitphasierten Arbeiten für das angegebene Datums‑Zeit‑Intervall.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Ruft die Menge der zeitphasierten Arbeit für das angegebene Datumszeitintervall ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Start des Datums‑Zeit‑Intervalls. |
| Ende | java.util.Date | Ende des Datums‑Zeit‑Intervalls. |
| timephasedDataType | byte | Typ der zu verwendenden zeitphasierten Daten. |

**Returns:**
double - Menge an zeitphasierten Arbeiten für das angegebene Datums‑Zeit‑Intervall.
### getUid() {#getUid--}
```
public final int getUid()
```


Liefert einen Wert von Uid.

**Returns:**
int - ein Wert von Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Ruft den Wert von Units ab.

**Returns:**
double - ein Wert von Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Ruft einen Wert ab, der angibt, ob UpdateNeeded gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob UpdateNeeded gesetzt ist oder nicht.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Ruft den Wert von VAC ab.

**Returns:**
double - ein Wert von VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Ermittelt einen Wert von Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Ruft den Wert von WorkContour ab.

**Returns:**
int - ein Wert von WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Ermittelt einen Wert von WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Ruft einen Wert ab, der anzeigt, dass diese Ressourcen-Zuweisung untergeordnete Elemente hat.

**Returns:**
boolean - Immer falsch.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Ruft einen Wert ab, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht.

**Returns:**
boolean - ein Wert, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Gibt einen Hashcode-Wert für die Instanz der Klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment) zurück.

**Returns:**
int - gibt einen Hashcode-Wert für dieses Objekt zurück.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Erzeugt eine Liste von zeitphasierten Daten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Das angegebene Startdatum. |
| Zeit | double | Die angegebene Arbeitszeit. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Der angegebene Arbeitskalender. |
| Liste | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | Die Liste der zeitphasierten Daten. |
| isWorking | boolean | Das angegebene Flag, das angibt, ob zeitphasierte Daten arbeiten oder nicht. |
| Typ | int | Der angegebene zeitphasierte Datentyp. |

**Returns:**
java.util.Date - Ein maximales Datum aus der Liste oder das Startdatum, wenn die Liste leer ist.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Setzt einen Wert von ACWP.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Setzt einen Wert von ActualCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Setzt einen Wert von ActualFinish.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von ActualFinish. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Setzt einen Wert von ActualStart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von ActualStart. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Setzt einen Wert, der angibt, ob Confirmed gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Confirmed gesetzt ist oder nicht. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Setzt einen Wert für Cost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Setzt einen Wert von CostRateTableType.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von CostRateTableType. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Setzt einen Wert von Delay.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Setzt eine Instanz der Klasse ExtendedAttributeCollection für dieses Objekt.

--------------------

Lesen wird nur für das XML-Format unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | eine Instanz der Klasse ExtendedAttributeCollection für dieses Objekt. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Setzt einen Wert für Finish.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Setzt einen Wert von FinishVariance.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Legt einen Wert fest, der angibt, ob FixedMaterial gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob FixedMaterial gesetzt ist oder nicht. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Legt einen Wert fest, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob HasFixedRateUnits gesetzt ist oder nicht. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Legt die eindeutige Kennung für diese Zuordnung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID | eindeutiger Bezeichner für diese Zuordnung. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Legt einen Wert für Hyperlink fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Legt einen Wert für HyperlinkAddress fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Legt einen Wert für HyperlinkSubAddress fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | ein Wert von HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Legt einen Wert für LevelingDelay fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Legt einen Wert fest, der angibt, ob LinkedFields gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob LinkedFields gesetzt ist oder nicht. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Legt Einheiten für die Zuweisung einer Materialressource mit variablem Materialverbrauch fest. Der variable Materialverbrauch bedeutet, dass sich die Menge der verwendeten Materialien proportional ändert, wenn die Zuweisungsdauer sich ändert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Einheiten | double | Anzahl der im Zeitraum angesammelten Einheiten. |
|  | rateScaleType | int | Zeitraum, in dem der Einheitswert angesammelt wird. |

--------------------

Zum Beispiel, um '123/Monat' festzulegen, sollte SetUnitsScaled(123D, RateScaleType.Month) aufgerufen werden. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Legt einen Wert fest, der angibt, ob Milestone gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Milestone gesetzt ist oder nicht. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Legt die Textnotizen im RTF-Format fest.

--------------------

Nur für MPP-Formate unterstützt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Textnotizen im RTF-Format. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Legt den Klartext der Notizen fest, der aus RTF-Daten extrahiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | der reine Text der Notizen, extrahiert aus RTF-Daten. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Setzt einen Wert, der angibt, ob Overallocated gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Overallocated gesetzt ist oder nicht. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Setzt einen Wert für OvertimeCost.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.math.BigDecimal | ein Wert von OvertimeCost. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Legt einen Wert für RateScale fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von RateScale. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


Die einer Aufgabe zugewiesene Ressource.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | die Ressource, die einer Aufgabe zugewiesen ist. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Legt einen Wert fest, der angibt, ob ResponsePending gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob ResponsePending gesetzt ist oder nicht. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Legt einen Wert für Resume fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Setzt einen Wert für SV.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Setzt einen Wert für Start.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Legt einen Wert für StartVariance fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Legt einen Wert für Stop fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | ein Wert von Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Legt einen Wert fest, der angibt, ob Summary gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob Summary gesetzt ist oder nicht. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


Die Aufgabe, der eine Ressource zugewiesen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | die Aufgabe, der eine Ressource zugewiesen ist. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Legt die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) fest, die Elemente von `TimephasedData` ([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | die Instanz der Klasse [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection), die Elemente von `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) enthält. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Setzt einen Wert für Uid.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Legt einen Wert für Units fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Legt einen Wert fest, der angibt, ob UpdateNeeded gesetzt ist oder nicht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ein Wert, der angibt, ob UpdateNeeded gesetzt ist oder nicht. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Legt einen Wert für VAC fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double | ein Wert von VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Setzt einen Wert für Work.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Legt einen Wert für WorkContour fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | ein Wert von WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Setzt einen Wert für WorkVariance.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ein Wert von WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Teilt die Aufgabe in zwei Teile.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| start | java.util.Date | Der Beginn der Arbeitsunterbrechung, nach dem gesplittet werden soll. |
| Abschluss | java.util.Date | Das Ende der Arbeitsunterbrechung, nach dem gesplittet werden soll. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Der Kalender, nach dem gesplittet werden soll. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Erzeugt eine Liste von zeitlich gestaffelten Daten basierend auf der Aufgabendauer und dem geplanten Startdatum.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Der Kalender, aus dem zeitphasenbezogene Daten erzeugt werden. |

### toString() {#toString--}
```
public String toString()
```


Gibt die kurze Zeichenkettenrepräsentation der Instanz der Klasse [ResourceAssignment](../../com.aspose.tasks/resourceassignment) zurück. Die genauen Details der Darstellung sind nicht spezifiziert und können sich ändern.

**Returns:**
java.lang.String - kurze Zeichenkette, die das Zuweisungsobjekt darstellt.

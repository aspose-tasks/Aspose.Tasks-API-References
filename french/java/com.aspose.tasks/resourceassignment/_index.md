---
title: "ResourceAssignment"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une affectation de ressource dans un projet."
type: docs
weight: 249
url: /fr/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Représente une affectation de ressource dans un projet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [delete()](#delete--) | Supprime l'affectation de ressources de la collection des affectations du projet. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Renvoie une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getACWP()](#getACWP--) | Obtient une valeur de ACWP. |
| [getActualCost()](#getActualCost--) | Obtient une valeur de ActualCost. |
| [getActualFinish()](#getActualFinish--) | Obtient une valeur de ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Obtient une valeur de ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Obtient une valeur de ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Obtient une valeur de ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Obtient une valeur de ActualStart. |
| [getActualWork()](#getActualWork--) | Obtient une valeur de ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Obtient une valeur de ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Obtient une valeur de AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Obtient une valeur de AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Obtient une valeur de BCWP. |
| [getBCWS()](#getBCWS--) | Obtient une valeur de BCWS. |
| [getBaselines()](#getBaselines--) | Obtient l'objet AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | Obtient une valeur de BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Obtient une valeur de BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Obtient une valeur de BudgetWork. |
| [getCV()](#getCV--) | Obtient une valeur de CV. |
| [getConfirmed()](#getConfirmed--) | Obtient une valeur indiquant si Confirmed est défini ou non. |
| [getCost()](#getCost--) | Obtient une valeur de Coût. |
| [getCostRateTableType()](#getCostRateTableType--) | Obtient une valeur de CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Obtient une valeur de CostVariance. |
| [getCreated()](#getCreated--) | Obtient une valeur de Created. |
| [getDelay()](#getDelay--) | Obtient une valeur de Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtient une instance de la classe ExtendedAttributeCollection pour cet objet. |
| [getFinish()](#getFinish--) | Obtient une valeur de Finish. |
| [getFinishVariance()](#getFinishVariance--) | Obtient une valeur de FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Obtient une valeur indiquant si FixedMaterial est défini ou non. |
| [getGuid()](#getGuid--) | Obtient l'identifiant unique pour cette affectation. |
| [getHyperlink()](#getHyperlink--) | Obtient une valeur de Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Obtient une valeur de HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Obtient une valeur de HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Obtient une valeur de LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Obtient une valeur indiquant si LinkedFields est défini ou non. |
| [getMilestone()](#getMilestone--) | Obtient une valeur indiquant si Milestone est défini ou non. |
| [getNotesRTF()](#getNotesRTF--) | Obtient les notes texte au format RTF. |
| [getNotesText()](#getNotesText--) | Obtient le texte brut des notes extrait des données RTF. |
| [getOverallocated()](#getOverallocated--) | Obtient une valeur indiquant si Overallocated est défini ou non. |
| [getOvertimeCost()](#getOvertimeCost--) | Obtient la valeur de OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Obtient la valeur de OvertimeWork. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent pour cette affectation. |
| [getPeakUnits()](#getPeakUnits--) | Obtient la valeur de PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Obtient la valeur de PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Obtient une valeur de RateScale. |
| [getRegularWork()](#getRegularWork--) | Obtient la valeur de RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Obtient la valeur de RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Obtient la valeur de RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Obtient la valeur de RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Obtient la valeur de RemainingWork. |
| [getResource()](#getResource--) | La ressource assignée à une tâche. |
| [getResponsePending()](#getResponsePending--) | Obtient une valeur indiquant si ResponsePending est défini ou non. |
| [getResume()](#getResume--) | Obtient une valeur de Resume. |
| [getSV()](#getSV--) | Obtient la valeur de SV. |
| [getStart()](#getStart--) | Obtient la valeur de Start. |
| [getStartVariance()](#getStartVariance--) | Obtient une valeur de StartVariance. |
| [getStop()](#getStop--) | Obtient une valeur de Stop. |
| [getSummary()](#getSummary--) | Obtient une valeur indiquant si Summary est défini ou non. |
| [getTask()](#getTask--) | La tâche à laquelle une ressource est assignée. |
| [getTimephasedData()](#getTimephasedData--) | Obtient l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant les éléments de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Renvoie l'objet [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) avec les instances de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) classe dans les dates de début et de fin données du [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Renvoie l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant les instances de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) classe dans les dates de début et de fin données du [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Obtient la quantité de travail temporel pour l'intervalle de date et d'heure spécifié. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Obtient la quantité de travail temporel pour l'intervalle de date et d'heure spécifié. |
| [getUid()](#getUid--) | Obtient la valeur de Uid. |
| [getUnits()](#getUnits--) | Obtient une valeur de Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Obtient une valeur indiquant si UpdateNeeded est défini ou non. |
| [getVAC()](#getVAC--) | Obtient une valeur de VAC. |
| [getWork()](#getWork--) | Obtient la valeur de Work. |
| [getWorkContour()](#getWorkContour--) | Obtient une valeur de WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Obtient une valeur de WorkVariance. |
| [hasChildren()](#hasChildren--) | Obtient une valeur indiquant que cette affectation de ressource possède des enfants. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Obtient une valeur indiquant si HasFixedRateUnits est défini ou non. |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Génère une liste de données temporelles phasées. |
| [setACWP(double value)](#setACWP-double-) | Définit une valeur de ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Définit une valeur de ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Définit une valeur pour ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Définit une valeur de ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Définit une valeur de ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Définit une valeur pour ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Définit une valeur de ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Définit une valeur de ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Définit une valeur de AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Définit une valeur de AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Définit une valeur de BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Définit une valeur de BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Définit une valeur de BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Définit une valeur de BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Définit une valeur de BudgetWork. |
| [setCV(double value)](#setCV-double-) | Définit une valeur de CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Définit une valeur indiquant si Confirmed est défini ou non. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Définit une valeur de Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Définit une valeur pour CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Définit une valeur de CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Définit une valeur de Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Définit une valeur pour Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Définit une instance de la classe ExtendedAttributeCollection pour cet objet. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Définit une valeur de Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Définit une valeur pour FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Définit une valeur indiquant si FixedMaterial est défini ou non. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Définit une valeur indiquant si HasFixedRateUnits est défini ou non. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Définit l'identifiant unique pour cette affectation. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Définit une valeur pour Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Définit une valeur pour HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Définit une valeur pour HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Définit une valeur pour LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Définit une valeur indiquant si LinkedFields est défini ou non. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Définit les unités pour l'affectation d'une ressource matérielle avec consommation variable de matériel. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Définit une valeur indiquant si Milestone est défini ou non. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Définit les notes texte au format RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Définit le texte brut des notes extrait des données RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Définit une valeur indiquant si Overallocated est défini ou non. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Définit une valeur de OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Définit une valeur de PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Définit une valeur de PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Définit une valeur pour RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Définit une valeur de RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Définit une valeur de RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Définit une valeur de RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Définit une valeur de RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | La ressource assignée à une tâche. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Définit une valeur indiquant si ResponsePending est défini ou non. |
| [setResume(Date value)](#setResume-java.util.Date-) | Définit une valeur de Resume. |
| [setSV(double value)](#setSV-double-) | Définit une valeur de SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Définit une valeur de Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Définit une valeur de StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Définit une valeur de Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Définit une valeur indiquant si Summary est défini ou non. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | La tâche à laquelle une ressource est assignée. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Définit l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant des éléments de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe. |
| [setUid(int value)](#setUid-int-) | Définit une valeur de Uid. |
| [setUnits(double value)](#setUnits-double-) | Définit une valeur de Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Définit une valeur indiquant si UpdateNeeded est défini ou non. |
| [setVAC(double value)](#setVAC-double-) | Définit une valeur de VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Définit une valeur de Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Définit une valeur de WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Définit une valeur de WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Divise la tâche en deux parties. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Génère une liste de données temporelles basée sur la durée de la tâche et la date de début prévue. |
| [toString()](#toString--) | Renvoie une représentation courte sous forme de chaîne de l'instance de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Asn](../../com.aspose.tasks/asn) pour obtenir la clé de propriété. |

**Returns:**
T - la valeur à laquelle la propriété est mappée dans ce conteneur.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Asn](../../com.aspose.tasks/asn) pour obtenir la clé de propriété. |
| val | T | la valeur. |

### delete() {#delete--}
```
public final void delete()
```


Supprime l'affectation de ressources de la collection des affectations du projet.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Renvoie une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | L'instance spécifiée de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment) à comparer avec cette instance. |

**Returns:**
booléen - **True** si l'instance spécifiée de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment) a la même valeur UID que cette instance ; sinon, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | L'objet à comparer avec cette instance. |

**Returns:**
booléen - **True** si o est un ResourceAssignment qui assigne la même ressource et la même tâche que cette instance ; sinon, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Obtient une valeur de ACWP.

**Returns:**
double - une valeur de ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Obtient une valeur de ActualCost.

**Returns:**
java.math.BigDecimal - une valeur de ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Obtient une valeur de ActualFinish.

**Returns:**
java.util.Date - une valeur de ActualFinish.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Obtient une valeur de ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - une valeur de ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Obtient une valeur de ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Obtient une valeur de ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Obtient une valeur de ActualStart.

**Returns:**
java.util.Date - une valeur de ActualStart.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Obtient une valeur de ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Obtient une valeur de ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Obtient une valeur de AssignmentOwner.

**Returns:**
java.lang.String - une valeur de AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Obtient une valeur de AssignmentOwnerGuid.

**Returns:**
java.lang.String - une valeur de AssignmentOwnerGuid.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Obtient une valeur de BCWP.

**Returns:**
double - une valeur de BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Obtient une valeur de BCWS.

**Returns:**
double - une valeur de BCWS.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


Obtient l'objet AssignmentBaselineCollection. La collection des valeurs de base associées à une affectation.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Obtient une valeur de BookingType.

**Returns:**
int - une valeur de BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Obtient une valeur de BudgetCost.

**Returns:**
java.math.BigDecimal - une valeur de BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Obtient une valeur de BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Obtient une valeur de CV.

**Returns:**
double - une valeur de CV.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Obtient une valeur indiquant si Confirmed est défini ou non.

**Returns:**
booléen - une valeur indiquant si Confirmed est défini ou non.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtient une valeur de Coût.

**Returns:**
java.math.BigDecimal - une valeur de Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Obtient une valeur de CostRateTableType.

**Returns:**
int - une valeur de CostRateTableType.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Obtient une valeur de CostVariance.

**Returns:**
double - une valeur de CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Obtient une valeur de Created.

**Returns:**
java.util.Date - une valeur de Created.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Obtient une valeur de Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Obtient une instance de la classe ExtendedAttributeCollection pour cet objet.

--------------------

Lecture prise en charge uniquement pour le format XML.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtient une valeur de Finish.

**Returns:**
java.util.Date - une valeur de Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Obtient une valeur de FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Obtient une valeur indiquant si FixedMaterial est défini ou non.

**Returns:**
booléen - une valeur indiquant si FixedMaterial est défini ou non.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtient l'identifiant unique pour cette affectation.

**Returns:**
java.util.UUID - identifiant unique pour cette affectation.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Obtient une valeur de Hyperlink.

**Returns:**
java.lang.String - une valeur de Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Obtient une valeur de HyperlinkAddress.

**Returns:**
java.lang.String - une valeur de HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Obtient une valeur de HyperlinkSubAddress.

**Returns:**
java.lang.String - une valeur de HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Réservé à un usage interne.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Obtient une valeur de LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Obtient une valeur indiquant si LinkedFields est défini ou non.

**Returns:**
boolean - une valeur indiquant si LinkedFields est défini ou non.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Obtient une valeur indiquant si Milestone est défini ou non.

**Returns:**
boolean - une valeur indiquant si Milestone est défini ou non.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Obtient les notes texte au format RTF.

--------------------

Pris en charge uniquement pour les formats MPP.

**Returns:**
java.lang.String - les notes texte au format RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Obtient le texte brut des notes extrait des données RTF.

**Returns:**
java.lang.String - texte brut des notes extrait des données RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Obtient une valeur indiquant si Overallocated est défini ou non.

**Returns:**
boolean - une valeur indiquant si Overallocated est défini ou non.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Obtient la valeur de OvertimeCost.

**Returns:**
java.math.BigDecimal - une valeur de OvertimeCost.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Obtient la valeur de OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Obtient le projet parent pour cette affectation.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Obtient la valeur de PeakUnits.

**Returns:**
double - une valeur de PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Obtient la valeur de PercentWorkComplete.

**Returns:**
int - une valeur de PercentWorkComplete.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Obtient une valeur de RateScale.

**Returns:**
int - une valeur de RateScale.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Obtient la valeur de RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Obtient la valeur de RemainingCost.

**Returns:**
java.math.BigDecimal - une valeur de RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Obtient la valeur de RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - une valeur de RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Obtient la valeur de RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Obtient la valeur de RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


La ressource assignée à une tâche.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Obtient une valeur indiquant si ResponsePending est défini ou non.

**Returns:**
boolean - une valeur indiquant si ResponsePending est défini ou non.
### getResume() {#getResume--}
```
public final Date getResume()
```


Obtient une valeur de Resume.

**Returns:**
java.util.Date - une valeur de Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Obtient la valeur de SV.

**Returns:**
double - une valeur de SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtient la valeur de Start.

**Returns:**
java.util.Date - une valeur de Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Obtient une valeur de StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Obtient une valeur de Stop.

**Returns:**
java.util.Date - une valeur de Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Obtient une valeur indiquant si Summary est défini ou non.

**Returns:**
boolean - une valeur indiquant si Summary est défini ou non.
### getTask() {#getTask--}
```
public final Task getTask()
```


La tâche à laquelle une ressource est assignée.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtient l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant les éléments de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Renvoie l'objet [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) avec les instances de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) classe dans les dates de début et de fin données du [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | La date de début des données à phase temporelle. |
| fin | java.util.Date | La date de fin des données à phase temporelle. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Renvoie l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant les instances de `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) classe dans les dates de début et de fin données du [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | La date de début des données à phase temporelle. |
| fin | java.util.Date | La date de fin des données à phase temporelle. |
| timephasedType | byte | Le type des données à phase temporelle ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Obtient la quantité de travail temporel pour l'intervalle de date et d'heure spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Début de l'intervalle de date et d'heure. |
| fin | java.util.Date | Fin de l'intervalle de date et d'heure. |

**Returns:**
double - quantité de travail phasé dans le temps pour l'intervalle de date et d'heure spécifié.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Obtient la quantité de travail temporel pour l'intervalle de date et d'heure spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Début de l'intervalle de date et d'heure. |
| fin | java.util.Date | Fin de l'intervalle de date et d'heure. |
| timephasedDataType | byte | Type des données phasées dans le temps à utiliser. |

**Returns:**
double - quantité de travail phasé dans le temps pour l'intervalle de date et d'heure spécifié.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtient la valeur de Uid.

**Returns:**
int - une valeur de Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Obtient une valeur de Units.

**Returns:**
double - une valeur de Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Obtient une valeur indiquant si UpdateNeeded est défini ou non.

**Returns:**
boolean - une valeur indiquant si UpdateNeeded est défini ou non.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Obtient une valeur de VAC.

**Returns:**
double - une valeur de VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtient la valeur de Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Obtient une valeur de WorkContour.

**Returns:**
int - une valeur de WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Obtient une valeur de WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Obtient une valeur indiquant que cette affectation de ressource possède des enfants.

**Returns:**
boolean - Toujours faux.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Obtient une valeur indiquant si HasFixedRateUnits est défini ou non.

**Returns:**
boolean - une valeur indiquant si HasFixedRateUnits est défini ou non.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Génère une liste de données temporelles phasées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | La date de début spécifiée. |
| time | double | Le temps de travail spécifié. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Le calendrier de travail spécifié. |
| liste | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | La liste des données à phases temporelles. |
| isWorking | booléen | Le drapeau spécifié qui indique si les données à phases temporelles sont en cours ou non. |
| type | int | Le type de données à phases temporelles spécifié. |

**Returns:**
java.util.Date - Une date maximale de la liste ou la date de début si la liste est vide.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Définit une valeur de ACWP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Définit une valeur de ActualCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Définit une valeur pour ActualFinish.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de ActualFinish. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Définit une valeur de ActualOvertimeCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Définit une valeur de ActualOvertimeWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Définit une valeur de ActualOvertimeWorkProtected.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de ActualOvertimeWorkProtected. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Définit une valeur pour ActualStart.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de ActualStart. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Définit une valeur de ActualWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Définit une valeur de ActualWorkProtected.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Définit une valeur de AssignmentOwner.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Définit une valeur de AssignmentOwnerGuid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de AssignmentOwnerGuid. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Définit une valeur de BCWP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Définit une valeur de BCWS.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Définit une valeur de BookingType.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de BookingType. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Définit une valeur de BudgetCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Définit une valeur de BudgetWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Définit une valeur de CV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de CV. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Définit une valeur indiquant si Confirmed est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si Confirmed est défini ou non. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Définit une valeur de Cost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Définit une valeur pour CostRateTableType.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de CostRateTableType. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Définit une valeur de CostVariance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Définit une valeur de Created.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Created. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Définit une valeur pour Delay.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Définit une instance de la classe ExtendedAttributeCollection pour cet objet.

--------------------

Lecture prise en charge uniquement pour le format XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | une instance de la classe ExtendedAttributeCollection pour cet objet. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Définit une valeur de Finish.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Définit une valeur pour FinishVariance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Définit une valeur indiquant si FixedMaterial est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si FixedMaterial est défini ou non. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Définit une valeur indiquant si HasFixedRateUnits est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si HasFixedRateUnits est défini ou non. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Définit l'identifiant unique pour cette affectation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID | identifiant unique pour cet affectation. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Définit une valeur pour Hyperlink.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Définit une valeur pour HyperlinkAddress.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Définit une valeur pour HyperlinkSubAddress.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Définit une valeur pour LevelingDelay.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Définit une valeur indiquant si LinkedFields est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si LinkedFields est défini ou non. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Définit les unités pour l'affectation d'une ressource matérielle avec consommation variable de matériel. La consommation variable de matériel signifie que, à mesure que la durée de l'affectation change, la quantité de matériaux utilisée change proportionnellement.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| unités | double | Nombre d'unités accumulées pendant la période. |
|  | rateScaleType | int | Période pendant laquelle la valeur de l'unité est accumulée. |

--------------------

Par exemple, pour définir '123/mois', SetUnitsScaled(123D, RateScaleType.Month) doit être appelé. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Définit une valeur indiquant si Milestone est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si le jalon est défini ou non. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Définit les notes texte au format RTF.

--------------------

Pris en charge uniquement pour les formats MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | les notes texte au format RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Définit le texte brut des notes extrait des données RTF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | texte brut des notes extrait des données RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Définit une valeur indiquant si Overallocated est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si Overallocated est défini ou non. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Définit une valeur de OvertimeCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de OvertimeCost. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Définit une valeur de OvertimeWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Définit une valeur de PeakUnits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Définit une valeur de PercentWorkComplete.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de PercentWorkComplete. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Définit une valeur pour RateScale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de RateScale. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Définit une valeur de RegularWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Définit une valeur de RemainingCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Définit une valeur de RemainingOvertimeCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Définit une valeur de RemainingOvertimeWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Définit une valeur de RemainingWork.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de RemainingWork. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


La ressource assignée à une tâche.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | la ressource assignée à une tâche. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Définit une valeur indiquant si ResponsePending est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si ResponsePending est défini ou non. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Définit une valeur de Resume.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Définit une valeur de SV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Définit une valeur de Start.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Définit une valeur de StartVariance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Définit une valeur de Stop.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Définit une valeur indiquant si Summary est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si Summary est défini ou non. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


La tâche à laquelle une ressource est assignée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | la tâche à laquelle une ressource est assignée. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Définit l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant des éléments de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) classe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | l'instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) contenant des éléments de `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Définit une valeur de Uid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Définit une valeur de Units.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur d'Unités. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Définit une valeur indiquant si UpdateNeeded est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si UpdateNeeded est défini ou non. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Définit une valeur de VAC.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Définit une valeur de Work.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Définit une valeur de WorkContour.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Définit une valeur de WorkVariance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Divise la tâche en deux parties.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | Le début de l'interruption de travail à utiliser pour la division. |
| fin | java.util.Date | La fin de l'interruption de travail à utiliser pour la division. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Le calendrier à utiliser pour la division. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Génère une liste de données temporelles basée sur la durée de la tâche et la date de début prévue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Le calendrier à partir duquel générer les données temporelles. |

### toString() {#toString--}
```
public String toString()
```


Renvoie une représentation sous forme de chaîne courte de l'instance de la classe [ResourceAssignment](../../com.aspose.tasks/resourceassignment). Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

**Returns:**
java.lang.String - chaîne courte qui représente l'objet d'affectation.

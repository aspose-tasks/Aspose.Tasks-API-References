---
title: "Resource"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une ressource dans un projet."
type: docs
weight: 248
url: /fr/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Représente une ressource dans un projet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [canLevel()](#canLevel--) | Obtient une valeur indiquant si CanLevel est défini ou non. |
| [delete()](#delete--) | Supprime une ressource et ses affectations du projet. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Renvoie une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [getACWP()](#getACWP--) | Obtient une valeur de ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Obtient une valeur de AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Obtient une valeur de ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Obtient une valeur de ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Obtient une valeur de ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Obtient une valeur de ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Obtient une valeur de ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Obtient une valeur de ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Obtient une valeur de ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Obtient une valeur de AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Obtient une valeur de AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Obtient une collection d'affectations de ressources pour cet objet. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Obtient l'instance de la classe [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Obtient une valeur de AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Obtient une valeur de AvailableTo. |
| [getBCWP()](#getBCWP--) | Obtient une valeur de BCWP. |
| [getBCWS()](#getBCWS--) | Obtient une valeur de BCWS. |
| [getBaselines()](#getBaselines--) | Obtient une instance de BaselineCollection pour cet objet. |
| [getBookingType()](#getBookingType--) | Obtient une valeur de BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Obtient une valeur de BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Obtient une valeur de BudgetWork. |
| [getCV()](#getCV--) | Obtient une valeur de CV. |
| [getCalendar()](#getCalendar--) | Obtient une valeur de Calendar. |
| [getCode()](#getCode--) | Obtient une valeur de Code. |
| [getCost()](#getCost--) | Obtient une valeur de Coût. |
| [getCostCenter()](#getCostCenter--) | Obtient une valeur de CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Obtient une valeur de CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Obtient une valeur de CostVariance. |
| [getCreated()](#getCreated--) | Obtient une valeur de Created. |
| [getEMailAddress()](#getEMailAddress--) | Obtient une valeur de EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Obtient les valeurs d'un attribut étendu. |
| [getFinish()](#getFinish--) | Obtient une valeur de Finish. |
| [getGroup()](#getGroup--) | Obtient une valeur de Group. |
| [getGuid()](#getGuid--) | Obtient une valeur de Guid. |
| [getHyperlink()](#getHyperlink--) | Obtient le titre ou le texte explicatif d'un hyperlien associé à une ressource. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Obtient l'adresse d'un hyperlien associé à une ressource. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Obtient l'emplacement spécifique dans un document d'un hyperlien associé à une ressource. |
| [getId()](#getId--) | Obtient une valeur de Id. |
| [getInactive()](#getInactive--) | Obtient une valeur indiquant si Inactive est défini ou non. |
| [getInitials()](#getInitials--) | Obtient une valeur de Initials. |
| [getItems()](#getItems--) | Obtient les ressources enfants. |
| [getMaterialLabel()](#getMaterialLabel--) | Obtient une valeur de MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Obtient une valeur de MaxUnits. |
| [getName()](#getName--) | Obtient une valeur de Name. |
| [getNotesRTF()](#getNotesRTF--) | Obtient une valeur de NotesRTF. |
| [getNotesText()](#getNotesText--) | Obtient une valeur de NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Obtient un objet OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | Obtient une valeur indiquant si Overallocated est défini ou non. |
| [getOvertimeCost()](#getOvertimeCost--) | Obtient la valeur de OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Obtient la valeur de OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Obtient la valeur de OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Obtient la valeur de OvertimeWork. |
| [getParentProject()](#getParentProject--) | Obtient le projet parent pour ce conteneur. |
| [getPeakUnits()](#getPeakUnits--) | Obtient la valeur de PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Obtient la valeur de PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Obtient la valeur de Phonetics. |
| [getRates()](#getRates--) | Obtient l'instance de la classe [RateCollection](../../com.aspose.tasks/ratecollection) pour cet objet. |
| [getRegularWork()](#getRegularWork--) | Obtient la valeur de RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Obtient la valeur de RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Obtient la valeur de RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Obtient la valeur de RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Obtient la valeur de RemainingWork. |
| [getSV()](#getSV--) | Obtient la valeur de SV. |
| [getStandardRate()](#getStandardRate--) | Obtient la valeur de StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Obtient la valeur de StandardRateFormat. |
| [getStart()](#getStart--) | Obtient la valeur de Start. |
| [getTimephasedData()](#getTimephasedData--) | Obtient une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Renvoie [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet avec les valeurs `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dans les dates de début et de fin données. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Renvoie une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet avec les valeurs `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dans les dates de début et de fin données du [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getType()](#getType--) | Obtient la valeur de Type. |
| [getUid()](#getUid--) | Obtient la valeur de Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Obtient la valeur de WindowsUserAccount. |
| [getWork()](#getWork--) | Obtient la valeur de Work. |
| [getWorkVariance()](#getWorkVariance--) | Obtient une valeur de WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Obtient une valeur de Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Renvoie une valeur de code de hachage pour l'instance de la classe [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Obtient une valeur indiquant si IsBudget est défini ou non. |
| [isCostResource()](#isCostResource--) | Obtient une valeur indiquant si IsCostResource est défini ou non. |
| [isEnterprise()](#isEnterprise--) | Obtient une valeur indiquant si IsEnterprise est défini ou non. |
| [isGeneric()](#isGeneric--) | Obtient une valeur indiquant si IsGeneric est défini ou non. |
| [isNull()](#isNull--) | Obtient une valeur indiquant si IsNull est défini ou non. |
| [isRoot()](#isRoot--) | Obtient le drapeau indiquant si la ressource est une ressource racine. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Obtient une valeur indiquant si IsTeamAssignmentPool est défini ou non. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur. |
| [setACWP(double value)](#setACWP-double-) | Définit une valeur de ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Définit une valeur de AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Définit une valeur de ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Définit une valeur de ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Définit une valeur de ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Définit une valeur de ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Définit une valeur de ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Définit une valeur de ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Définit une valeur de AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Définit une valeur de AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Définit une valeur de AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Définit une valeur de AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Définit une valeur de BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Définit une valeur de BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Définit une valeur de BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si IsBudget est défini ou non. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Définit une valeur de BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Définit une valeur de BudgetWork. |
| [setCV(double value)](#setCV-double-) | Définit une valeur de CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Définit une valeur de Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si CanLevel est défini ou non. |
| [setCode(String value)](#setCode-java.lang.String-) | Définit une valeur de Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Définit une valeur de Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Définit une valeur de CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Définit une valeur de CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si IsCostResource est défini ou non. |
| [setCostVariance(double value)](#setCostVariance-double-) | Définit une valeur de CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Définit une valeur de Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Définit une valeur de EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si IsEnterprise est défini ou non. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Définit une valeur de Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si IsGeneric est défini ou non. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Définit une valeur de Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Définit une valeur de Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Définit le titre ou le texte explicatif d'un hyperlien associé à une ressource. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Définit l'adresse d'un hyperlien associé à une ressource. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Définit l'emplacement spécifique dans un document d'un hyperlien associé à une ressource. |
| [setId(int value)](#setId-int-) | Définit une valeur de Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si Inactive est défini ou non. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Définit une valeur de Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Définit une valeur de MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Définit une valeur de MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Définit une valeur de Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Définit une valeur de NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Définit une valeur de NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si IsNull est défini ou non. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Définit une valeur indiquant si Overallocated est défini ou non. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Définit une valeur de OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Définit une valeur de OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Définit une valeur de OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Définit une valeur de PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Définit une valeur de PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Définit une valeur de Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Définit une valeur de RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Définit une valeur de RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Définit une valeur de RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Définit une valeur de RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Définit une valeur de RemainingWork. |
| [setSV(double value)](#setSV-double-) | Définit une valeur de SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Définit une valeur de StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Définit une valeur de StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Définit une valeur de Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Définit une valeur indiquant si IsTeamAssignmentPool est défini ou non. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Définit une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet. |
| [setType(int value)](#setType-int-) | Définit une valeur de Type. |
| [setUid(int value)](#setUid-int-) | Définit une valeur de Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Définit une valeur de WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Définit une valeur de Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Définit une valeur de WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Définit une valeur de Workgroup. |
| [toString()](#toString--) | Renvoie la représentation courte sous forme de chaîne de l'instance de la classe [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Rsc](../../com.aspose.tasks/rsc) pour obtenir la clé de propriété. |

**Returns:**
T - la valeur à laquelle la propriété est mappée dans ce conteneur.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | la clé de propriété spécifiée. [Rsc](../../com.aspose.tasks/rsc) pour obtenir la clé de propriété. |
| val | T | la valeur. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Obtient une valeur indiquant si CanLevel est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Supprime une ressource et ses affectations du projet.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Renvoie une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | L'instance spécifiée de la classe [Resource](../../com.aspose.tasks/resource) à comparer avec cette instance. |

**Returns:**
booléen - **True** si l'instance spécifiée de la classe [Resource](../../com.aspose.tasks/resource) a la même valeur Uid que cette instance ; sinon, **false**.
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
booléen - **True** si l'objet spécifié est une Resource qui a la même valeur Uid que cette instance ; sinon, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Obtient une valeur de ACWP.

**Returns:**
double - une valeur de ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Obtient une valeur de AccrueAt.

**Returns:**
int - une valeur de AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Obtient une valeur de ActiveDirectoryGuid.

**Returns:**
java.lang.String - une valeur de ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Obtient une valeur de ActualCost.

**Returns:**
java.math.BigDecimal - une valeur de ActualCost.
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
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Obtient une collection d'affectations de ressources pour cet objet.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Obtient l'instance de la classe [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). La collection de périodes pendant lesquelles une ressource est disponible.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Obtient une valeur de AvailableFrom.

**Returns:**
java.util.Date - une valeur de AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Obtient une valeur de AvailableTo.

**Returns:**
java.util.Date - une valeur de AvailableTo.
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
public final BaselineCollection getBaselines()
```


Obtient une instance de BaselineCollection pour cet objet. Les valeurs de référence pour une ressource.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
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
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Obtient une valeur de Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Obtient une valeur de Code.

**Returns:**
java.lang.String - une valeur de Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Obtient une valeur de Coût.

**Returns:**
java.math.BigDecimal - une valeur de Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Obtient une valeur de CostCenter.

**Returns:**
java.lang.String - une valeur de CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Obtient une valeur de CostPerUse.

**Returns:**
java.math.BigDecimal - une valeur de CostPerUse.
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
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Obtient une valeur de EMailAddress.

**Returns:**
java.lang.String - une valeur de EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Obtient les valeurs d'un attribut étendu.

--------------------

Deux éléments de données sont nécessaires - un pointeur vers la table d'attributs étendue qui est spécifié soit par l'ID unique ou le Field ID, et la valeur qui est spécifiée soit avec la valeur, ou un pointeur vers la liste de valeurs.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Obtient une valeur de Finish.

**Returns:**
java.util.Date - une valeur de Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Obtient une valeur de Group.

**Returns:**
java.lang.String - une valeur de Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Obtient une valeur de Guid.

**Returns:**
java.lang.String - une valeur de Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Obtient le titre ou le texte explicatif d'un hyperlien associé à une ressource.

**Returns:**
java.lang.String - le titre ou le texte explicatif d'un hyperlien associé à une ressource.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Obtient l'adresse d'un hyperlien associé à une ressource.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

**Returns:**
java.lang.String - l'adresse d'un hyperlien associé à une ressource.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Obtient l'emplacement spécifique dans un document d'un hyperlien associé à une ressource.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

**Returns:**
java.lang.String - l'emplacement spécifique dans un document d'un hyperlien associé à une ressource.
### getId() {#getId--}
```
public final int getId()
```


Obtient une valeur de Id.

**Returns:**
int - une valeur de Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Obtient une valeur indiquant si Inactive est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Obtient une valeur de Initials.

**Returns:**
java.lang.String - une valeur de Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Obtient les ressources enfants.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - ressources enfants.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Obtient une valeur de MaterialLabel.

**Returns:**
java.lang.String - une valeur de MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Obtient une valeur de MaxUnits.

**Returns:**
double - une valeur de MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Obtient une valeur de Name.

**Returns:**
java.lang.String - une valeur de Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Obtient une valeur de NotesRTF.

**Returns:**
java.lang.String - une valeur de NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Obtient une valeur de NotesText.

**Returns:**
java.lang.String - une valeur de NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Obtient un objet OutlineCodeCollection. La valeur d'un code de plan.

--------------------

Deux éléments de données sont nécessaires - un pointeur vers la table de code de plan spécifiée par le FieldID, et la valeur qui est spécifiée soit par le ValueID soit par le pointeur ValueGUID vers la liste de valeurs.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Obtient une valeur indiquant si Overallocated est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Obtient la valeur de OvertimeCost.

**Returns:**
java.math.BigDecimal - une valeur de OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Obtient la valeur de OvertimeRate.

**Returns:**
java.math.BigDecimal - une valeur de OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Obtient la valeur de OvertimeRateFormat.

**Returns:**
int - une valeur de OvertimeRateFormat.
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


Obtient le projet parent pour ce conteneur.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
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
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Obtient la valeur de Phonetics.

**Returns:**
java.lang.String - une valeur de Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Obtient l'instance de la classe [RateCollection](../../com.aspose.tasks/ratecollection) pour cet objet. La collection de périodes et de taux associés à chacun.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
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
### getSV() {#getSV--}
```
public final double getSV()
```


Obtient la valeur de SV.

**Returns:**
double - une valeur de SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Obtient la valeur de StandardRate.

**Returns:**
java.math.BigDecimal - une valeur de StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Obtient la valeur de StandardRateFormat.

**Returns:**
int - une valeur de StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Obtient la valeur de Start.

**Returns:**
java.util.Date - une valeur de Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Obtient une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet.

--------------------

Lecture prise en charge uniquement pour le format XML.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Renvoie [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet avec les valeurs `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dans les dates de début et de fin données.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | La date de début pour les données temporelles. |
| fin | java.util.Date | La date de fin des données à phase temporelle. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Renvoie une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet avec les valeurs `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dans les dates de début et de fin données du [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| début | java.util.Date | La date de début des données à phase temporelle. |
| fin | java.util.Date | La date de fin des données à phase temporelle. |
| timephasedType | byte | Le type des données à phase temporelle ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Obtient la valeur de Type.

**Returns:**
int - une valeur de Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Obtient la valeur de Uid.

**Returns:**
int - une valeur de Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Obtient la valeur de WindowsUserAccount.

**Returns:**
java.lang.String - une valeur de WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Obtient la valeur de Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Obtient une valeur de WorkVariance.

**Returns:**
double - une valeur de WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Obtient une valeur de Workgroup.

**Returns:**
int - une valeur de Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Réservé à un usage interne.

**Returns:**
booléen - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Renvoie une valeur de code de hachage pour l'instance de la classe [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - renvoie une valeur de code de hachage pour cet objet.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Obtient une valeur indiquant si IsBudget est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Obtient une valeur indiquant si IsCostResource est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Obtient une valeur indiquant si IsEnterprise est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Obtient une valeur indiquant si IsGeneric est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Obtient une valeur indiquant si IsNull est défini ou non.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Obtient le drapeau indiquant si la ressource est une ressource racine. La ressource racine est une ressource spéciale destinée à prendre en charge les éléments internes des formats de MS Project et n'est pas destinée à être utilisée directement dans le code de l'utilisateur.

**Returns:**
boolean - le drapeau indiquant si la ressource est une ressource racine.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Obtient une valeur indiquant si IsTeamAssignmentPool est défini ou non.

**Returns:**
boolean - une valeur indiquant si IsTeamAssignmentPool est défini ou non.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | la clé de propriété spécifiée. [Rsc](../../com.aspose.tasks/rsc) pour obtenir la clé de propriété. |
| val | java.util.Date | la valeur. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Définit une valeur de ACWP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Définit une valeur de AccrueAt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Définit une valeur de ActiveDirectoryGuid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Définit une valeur de ActualCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de ActualCost. |

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

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Définit une valeur de AvailableFrom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Définit une valeur de AvailableTo.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de AvailableTo. |

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

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Définit une valeur indiquant si IsBudget est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si IsBudget est défini ou non. |

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

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Définit une valeur de Calendar.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | une valeur de Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Définit une valeur indiquant si CanLevel est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si CanLevel est défini ou non. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Définit une valeur de Code.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Définit une valeur de Cost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Définit une valeur de CostCenter.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Définit une valeur de CostPerUse.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Définit une valeur indiquant si IsCostResource est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si IsCostResource est défini ou non. |

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

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Définit une valeur de EMailAddress.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Définit une valeur indiquant si IsEnterprise est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si IsEnterprise est défini ou non. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Définit une valeur de Finish.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Définit une valeur indiquant si IsGeneric est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si IsGeneric est défini ou non. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Définit une valeur de Group.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Définit une valeur de Guid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Définit le titre ou le texte explicatif d'un hyperlien associé à une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le titre ou le texte explicatif d'un hyperlien associé à une ressource. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Définit l'adresse d'un hyperlien associé à une ressource.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | l'adresse d'un hyperlien associé à une ressource. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Définit l'emplacement spécifique dans un document d'un hyperlien associé à une ressource.

--------------------

L'adresse complète (Hyperlink Href dans Microsoft Project) de l'hyperlien est une concaténation de HyperlinkAddress et HyperlinkSubAddress.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | l'emplacement spécifique dans un document d'un hyperlien associé à une ressource. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Définit une valeur de Id.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Définit une valeur indiquant si Inactive est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si Inactive est défini ou non. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Définit une valeur de Initials.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Définit une valeur de MaterialLabel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Définit une valeur de MaxUnits.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Définit une valeur de Name.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Définit une valeur de NotesRTF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Définit une valeur de NotesText.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Définit une valeur indiquant si IsNull est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si IsNull est défini ou non. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Définit une valeur indiquant si Overallocated est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | une valeur indiquant si Overallocated est défini ou non. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Définit une valeur de OvertimeCost.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Définit une valeur de OvertimeRate.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Définit une valeur de OvertimeRateFormat.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de OvertimeRateFormat. |

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

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Définit une valeur de Phonetics.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de Phonetics. |

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

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Définit une valeur de SV.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Définit une valeur de StandardRate.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | une valeur de StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Définit une valeur de StandardRateFormat.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Définit une valeur de Start.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une valeur de Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Définit une valeur indiquant si IsTeamAssignmentPool est défini ou non.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si IsTeamAssignmentPool est défini ou non. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Définit une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet.

--------------------

Lecture prise en charge uniquement pour le format XML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | une instance de la classe [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) pour cet objet. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Définit une valeur de Type.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Définit une valeur de Uid.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Définit une valeur de WindowsUserAccount.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | une valeur de WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Définit une valeur de Work.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | une valeur de Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Définit une valeur de WorkVariance.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double | une valeur de WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Définit une valeur de Workgroup.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur de Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Renvoie une représentation sous forme de chaîne courte de l'instance de la classe [Resource](../../com.aspose.tasks/resource). Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

**Returns:**
java.lang.String - chaîne courte qui représente l'objet ressource.

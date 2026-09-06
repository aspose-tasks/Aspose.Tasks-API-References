---
title: "Resource"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projede bir kaynağı temsil eder."
type: docs
weight: 248
url: /tr/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Projede bir kaynağı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Bu konteynerde özelliğin eşlendiği değeri döndürür. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Belirtilen özelliği bu konteynerde belirtilen değere eşler. |
| [canLevel()](#canLevel--) | CanLevel'in ayarlanıp ayarlanmadığını gösteren bir değeri alır. |
| [delete()](#delete--) | Bir kaynağı ve atamalarını projeden siler. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Bu örneğin, belirtilen [Resource](../../com.aspose.tasks/resource) sınıfının bir örneğine eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getACWP()](#getACWP--) | ACWP değerini alır. |
| [getAccrueAt()](#getAccrueAt--) | AccrueAt değerini alır. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | ActiveDirectoryGuid değerini alır. |
| [getActualCost()](#getActualCost--) | ActualCost değerini alır. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost değerini alır. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork değerini alır. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected değerini alır. |
| [getActualWork()](#getActualWork--) | ActualWork değerini alır. |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected değerini alır. |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner değerini alır. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid değerini alır. |
| [getAssignments()](#getAssignments--) | Bu nesne için kaynak atamalarının bir koleksiyonunu alır. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) sınıfının örneğini alır. |
| [getAvailableFrom()](#getAvailableFrom--) | AvailableFrom değerini alır. |
| [getAvailableTo()](#getAvailableTo--) | AvailableTo değerini alır. |
| [getBCWP()](#getBCWP--) | BCWP değerini alır. |
| [getBCWS()](#getBCWS--) | BCWS değerini alır. |
| [getBaselines()](#getBaselines--) | Bu nesne için bir BaselineCollection örneğini alır. |
| [getBookingType()](#getBookingType--) | BookingType değerini alır. |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost değerini alır. |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork değerini alır. |
| [getCV()](#getCV--) | CV değerini alır. |
| [getCalendar()](#getCalendar--) | Calendar değerini alır. |
| [getCode()](#getCode--) | Code değerini alır. |
| [getCost()](#getCost--) | Cost değerini alır. |
| [getCostCenter()](#getCostCenter--) | CostCenter değerini alır. |
| [getCostPerUse()](#getCostPerUse--) | CostPerUse değerini alır. |
| [getCostVariance()](#getCostVariance--) | CostVariance değerini alır. |
| [getCreated()](#getCreated--) | Created değerini alır. |
| [getEMailAddress()](#getEMailAddress--) | EMailAddress değerini alır. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Genişletilmiş bir niteliğin değerlerini alır. |
| [getFinish()](#getFinish--) | Finish değerini alır. |
| [getGroup()](#getGroup--) | Group değerini alır. |
| [getGuid()](#getGuid--) | Guid değerini alır. |
| [getHyperlink()](#getHyperlink--) | Bir kaynakla ilişkili bir köprü için başlığı veya açıklayıcı metni alır. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Bir kaynakla ilişkili bir köprü için adresi alır. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Bir kaynakla ilişkili bir köprüdeki bir belgede belirli konumu alır. |
| [getId()](#getId--) | Id değerini alır. |
| [getInactive()](#getInactive--) | Inactive'in ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [getInitials()](#getInitials--) | Initials değerini alır. |
| [getItems()](#getItems--) | Alt kaynakları alır. |
| [getMaterialLabel()](#getMaterialLabel--) | MaterialLabel değerini alır. |
| [getMaxUnits()](#getMaxUnits--) | MaxUnits değerini alır. |
| [getName()](#getName--) | Name değerini alır. |
| [getNotesRTF()](#getNotesRTF--) | NotesRTF değerini alır. |
| [getNotesText()](#getNotesText--) | NotesText değerini alır. |
| [getOutlineCode()](#getOutlineCode--) | OutlineCodeCollection nesnesini alır. |
| [getOverallocated()](#getOverallocated--) | Overallocated'in ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost değerini alır. |
| [getOvertimeRate()](#getOvertimeRate--) | OvertimeRate değerini alır. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | OvertimeRateFormat değerini alır. |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork değerini alır. |
| [getParentProject()](#getParentProject--) | Bu kapsayıcı için üst projeyi alır. |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits değerini alır. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete değerini alır. |
| [getPhonetics()](#getPhonetics--) | Phonetics değerini alır. |
| [getRates()](#getRates--) | Bu nesne için [RateCollection](../../com.aspose.tasks/ratecollection) sınıfının bir örneğini alır. |
| [getRegularWork()](#getRegularWork--) | RegularWork değerini alır. |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost değerini alır. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost değerini alır. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork değerini alır. |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork değerini alır. |
| [getSV()](#getSV--) | SV değerini alır. |
| [getStandardRate()](#getStandardRate--) | StandardRate değerini alır. |
| [getStandardRateFormat()](#getStandardRateFormat--) | StandardRateFormat değerini alır. |
| [getStart()](#getStart--) | Start değerini alır. |
| [getTimephasedData()](#getTimephasedData--) | Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini alır. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfını, verilen başlangıç ve bitiş tarihleri içinde `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) değerleriyle döndürür. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini, belirtilen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) içinde verilen başlangıç ve bitiş tarihleri arasında `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) değerleriyle döndürür. |
| [getType()](#getType--) | Type değerini alır. |
| [getUid()](#getUid--) | Uid değerini alır. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | WindowsUserAccount değerini alır. |
| [getWork()](#getWork--) | Work değerini alır. |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance değerini alır. |
| [getWorkgroup()](#getWorkgroup--) | Workgroup değerini alır. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | [Resource](../../com.aspose.tasks/resource) sınıfının örneği için bir hash kod değeri döndürür. |
| [isBudget()](#isBudget--) | IsBudget ayarlı olup olmadığını gösteren değeri alır. |
| [isCostResource()](#isCostResource--) | IsCostResource ayarlı olup olmadığını gösteren değeri alır. |
| [isEnterprise()](#isEnterprise--) | IsEnterprise ayarlı olup olmadığını gösteren değeri alır. |
| [isGeneric()](#isGeneric--) | IsGeneric ayarlı olup olmadığını gösteren değeri alır. |
| [isNull()](#isNull--) | IsNull ayarlı olup olmadığını gösteren değeri alır. |
| [isRoot()](#isRoot--) | Kaynağın kök kaynak olup olmadığını gösteren bayrağı alır. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | IsTeamAssignmentPool ayarlı olup olmadığını gösteren değeri alır. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Belirtilen özelliği bu konteynerde belirtilen değere eşler. |
| [setACWP(double value)](#setACWP-double-) | ACWP değerini ayarlar. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | AccrueAt değerini ayarlar. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | ActiveDirectoryGuid değerini ayarlar. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost değerini ayarlar. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost değerini ayarlar. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork değerini ayarlar. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected değerini ayarlar. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork değerini ayarlar. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected değerini ayarlar. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner değerini ayarlar. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid değerini ayarlar. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | AvailableFrom değerini ayarlar. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | AvailableTo değerini ayarlar. |
| [setBCWP(double value)](#setBCWP-double-) | BCWP değerini ayarlar. |
| [setBCWS(double value)](#setBCWS-double-) | BCWS değerini ayarlar. |
| [setBookingType(int value)](#setBookingType-int-) | BookingType'in değerini ayarlar. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | IsBudget'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost'in değerini ayarlar. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork'in değerini ayarlar. |
| [setCV(double value)](#setCV-double-) | CV'in değerini ayarlar. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Calendar'ın değerini ayarlar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | CanLevel'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setCode(String value)](#setCode-java.lang.String-) | Code'un değerini ayarlar. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost'un değerini ayarlar. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | CostCenter'ın değerini ayarlar. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | CostPerUse'un değerini ayarlar. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | IsCostResource'un ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance'ın değerini ayarlar. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created'ın değerini ayarlar. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | EMailAddress'in değerini ayarlar. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | IsEnterprise'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish'in değerini ayarlar. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | IsGeneric'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Group'un değerini ayarlar. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Guid'in değerini ayarlar. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Bir kaynakla ilişkili bir köprünün başlığını veya açıklayıcı metnini ayarlar. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Bir kaynakla ilişkili bir köprünün adresini ayarlar. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Bir kaynakla ilişkili bir köprünün bir belgedeki belirli konumunu ayarlar. |
| [setId(int value)](#setId-int-) | Id'nin değerini ayarlar. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Inactive'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Initials'in değerini ayarlar. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | MaterialLabel'in değerini ayarlar. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | MaxUnits'in değerini ayarlar. |
| [setName(String value)](#setName-java.lang.String-) | Name'in değerini ayarlar. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | NotesRTF'in değerini ayarlar. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | NotesText'in değerini ayarlar. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | IsNull'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Overallocated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost'in değerini ayarlar. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | OvertimeRate'in değerini ayarlar. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | OvertimeRateFormat'in değerini ayarlar. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork'in değerini ayarlar. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits'in değerini ayarlar. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete'in değerini ayarlar. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Phonetics'in değerini ayarlar. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork'in değerini ayarlar. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost'in değerini ayarlar. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost'in değerini ayarlar. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork'in değerini ayarlar. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork'in değerini ayarlar. |
| [setSV(double value)](#setSV-double-) | SV'in değerini ayarlar. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | StandardRate'in değerini ayarlar. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | StandardRateFormat'in değerini ayarlar. |
| [setStart(Date value)](#setStart-java.util.Date-) | Start'in değerini ayarlar. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | IsTeamAssignmentPool'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini ayarlar. |
| [setType(int value)](#setType-int-) | Type değerini ayarlar. |
| [setUid(int value)](#setUid-int-) | Uid değerini ayarlar. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | WindowsUserAccount değerini ayarlar. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work değerini ayarlar. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | WorkVariance değerini ayarlar. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Workgroup değerini ayarlar. |
| [toString()](#toString--) | [Resource](../../com.aspose.tasks/resource) sınıfının örneğinin kısa dize temsilini döndürür. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Bu konteynerde özelliğin eşlendiği değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | belirtilen özellik anahtarı. Özellik anahtarını almak için [Rsc](../../com.aspose.tasks/rsc). |

**Returns:**
T - bu kapsayıcıda özelliğin eşlendiği değer.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Belirtilen özelliği bu konteynerde belirtilen değere eşler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | belirtilen özellik anahtarı. Özellik anahtarını almak için [Rsc](../../com.aspose.tasks/rsc). |
| değer. | T | değer. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


CanLevel'in ayarlanıp ayarlanmadığını gösteren bir değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Bir kaynağı ve atamalarını projeden siler.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Bu örneğin, belirtilen [Resource](../../com.aspose.tasks/resource) sınıfının bir örneğine eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | Bu örnek ile karşılaştırmak için belirtilen [Resource](../../com.aspose.tasks/resource) sınıfı örneği. |

**Returns:**
boolean - **True** ise belirtilen [Resource](../../com.aspose.tasks/resource) sınıfı örneği bu örnek ile aynı Uid değerine sahiptir; aksi takdirde **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnek ile karşılaştırılacak nesne. |

**Returns:**
boolean - **True** ise belirtilen nesne, bu örnek ile aynı Uid değerine sahip bir Resource'dur; aksi takdirde **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP değerini alır.

**Returns:**
double - ACWP değerini.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


AccrueAt değerini alır.

**Returns:**
int - AccrueAt değerini.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


ActiveDirectoryGuid değerini alır.

**Returns:**
java.lang.String - ActiveDirectoryGuid değerini.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost değerini alır.

**Returns:**
java.math.BigDecimal - ActualCost değerini.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost değerini alır.

**Returns:**
java.math.BigDecimal - ActualOvertimeCost değerini.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner değerini alır.

**Returns:**
java.lang.String - AssignmentOwner değerini.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid değerini alır.

**Returns:**
java.lang.String - AssignmentOwnerGuid değerini.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Bu nesne için kaynak atamalarının bir koleksiyonunu alır.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) sınıfının bir örneğini alır. Bir kaynağın mevcut olduğu dönemlerin koleksiyonu.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


AvailableFrom değerini alır.

**Returns:**
java.util.Date - AvailableFrom değerinin bir değeri.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


AvailableTo değerini alır.

**Returns:**
java.util.Date - AvailableTo değerinin bir değeri.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP değerini alır.

**Returns:**
double - BCWP değerinin bir değeri.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS değerini alır.

**Returns:**
double - BCWS değerinin bir değeri.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Bu nesne için bir BaselineCollection örneği alır. Bir kaynak için temel değerler.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType değerini alır.

**Returns:**
int - BookingType değerinin bir değeri.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost değerini alır.

**Returns:**
java.math.BigDecimal - BudgetCost değerinin bir değeri.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV değerini alır.

**Returns:**
double - CV değerinin bir değeri.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Calendar değerini alır.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Code değerini alır.

**Returns:**
java.lang.String - Code değerinin bir değeri.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost değerini alır.

**Returns:**
java.math.BigDecimal - Cost değerinin bir değeri.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


CostCenter değerini alır.

**Returns:**
java.lang.String - CostCenter değerinin bir değeri.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


CostPerUse değerini alır.

**Returns:**
java.math.BigDecimal - CostPerUse değerinin bir değeri.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


CostVariance değerini alır.

**Returns:**
double - CostVariance değerinin bir değeri.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Created değerini alır.

**Returns:**
java.util.Date - Created değerinin bir değeri.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


EMailAddress değerini alır.

**Returns:**
java.lang.String - EMailAddress değerinin bir değeri.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Genişletilmiş bir niteliğin değerlerini alır.

--------------------

İki veri parçası gereklidir - benzersiz kimlik ya da Alan kimliğiyle belirtilen genişletilmiş öznitelik tablosuna bir işaretçi ve değerin ya değerle ya da değer listesine bir işaretçiyle belirtilmesi.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish değerini alır.

**Returns:**
java.util.Date - Finish değerinin bir değeri.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Group değerini alır.

**Returns:**
java.lang.String - Group değerinin bir değeri.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Guid değerini alır.

**Returns:**
java.lang.String - Guid değerinin bir değeri.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Bir kaynakla ilişkili bir köprü için başlığı veya açıklayıcı metni alır.

**Returns:**
java.lang.String - bir kaynakla ilişkili köprünün başlığı veya açıklayıcı metni.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Bir kaynakla ilişkili bir köprü için adresi alır.

--------------------

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

**Returns:**
java.lang.String - bir kaynakla ilişkili köprünün adresi.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Bir kaynakla ilişkili bir köprüdeki bir belgede belirli konumu alır.

--------------------

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

**Returns:**
java.lang.String - bir kaynakla ilişkili köprünün bir belgede belirli konumu.
### getId() {#getId--}
```
public final int getId()
```


Id değerini alır.

**Returns:**
int - Id değerinin bir değeri.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Inactive'in ayarlanıp ayarlanmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Initials değerini alır.

**Returns:**
java.lang.String - Initials değerinin bir değeri.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Alt kaynakları alır.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - alt kaynaklar.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


MaterialLabel değerini alır.

**Returns:**
java.lang.String - MaterialLabel'in bir değeri.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


MaxUnits değerini alır.

**Returns:**
double - MaxUnits'in bir değeri.
### getName() {#getName--}
```
public final String getName()
```


Name değerini alır.

**Returns:**
java.lang.String - Name'in bir değeri.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


NotesRTF değerini alır.

**Returns:**
java.lang.String - NotesRTF'in bir değeri.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


NotesText değerini alır.

**Returns:**
java.lang.String - NotesText'in bir değeri.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Bir OutlineCodeCollection nesnesi alır. Bir taslak kodunun değeri.

--------------------

İki veri parçası gereklidir - FieldID ile belirtilen taslak kod tablosuna bir işaretçi ve ValueID veya ValueGUID işaretçisiyle belirtilen değer listesine bir işaretçi.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Overallocated'in ayarlanıp ayarlanmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost değerini alır.

**Returns:**
java.math.BigDecimal - OvertimeCost'in bir değeri.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


OvertimeRate değerini alır.

**Returns:**
java.math.BigDecimal - OvertimeRate'in bir değeri.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


OvertimeRateFormat değerini alır.

**Returns:**
int - OvertimeRateFormat'ın bir değeri.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


OvertimeWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Bu kapsayıcı için üst projeyi alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


PeakUnits değerini alır.

**Returns:**
double - PeakUnits'in bir değeri.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


PercentWorkComplete değerini alır.

**Returns:**
int - PercentWorkComplete'in bir değeri.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Phonetics değerini alır.

**Returns:**
java.lang.String - Phonetics'in bir değeri.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Bu nesne için [RateCollection](../../com.aspose.tasks/ratecollection) sınıfının bir örneğini alır. Her biriyle ilişkili dönemler ve oranların koleksiyonu.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


RegularWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


RemainingCost değerini alır.

**Returns:**
java.math.BigDecimal - RemainingCost'in bir değeri.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


RemainingOvertimeCost değerini alır.

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost'in bir değeri.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


RemainingOvertimeWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


RemainingWork değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


SV değerini alır.

**Returns:**
double - SV'nin bir değeri.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


StandardRate değerini alır.

**Returns:**
java.math.BigDecimal - StandardRate'in bir değeri.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


StandardRateFormat değerini alır.

**Returns:**
int - StandardRateFormat'ın bir değeri.
### getStart() {#getStart--}
```
public final Date getStart()
```


Start değerini alır.

**Returns:**
java.util.Date - Start'ın bir değeri.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini alır.

--------------------

Okuma yalnızca XML formatı için desteklenir.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfını, verilen başlangıç ve bitiş tarihleri içinde `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) değerleriyle döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Zaman aşamalı veriler için başlangıç tarihi. |
| bitiş | java.util.Date | Zaman aşamalı veriler için bitiş tarihi. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini, belirtilen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) içinde verilen başlangıç ve bitiş tarihleri arasında `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) değerleriyle döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Zaman aşamalı veriler için başlangıç tarihi. |
| bitiş | java.util.Date | Zaman aşamalı veriler için bitiş tarihi. |
| timephasedType | byte | Zaman aşamalı verilerin türü ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Type değerini alır.

**Returns:**
int - Type değerinin bir değeri.
### getUid() {#getUid--}
```
public final int getUid()
```


Uid değerini alır.

**Returns:**
int - Uid değerinin bir değeri.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


WindowsUserAccount değerini alır.

**Returns:**
java.lang.String - WindowsUserAccount değerinin bir değeri.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


WorkVariance değerini alır.

**Returns:**
double - WorkVariance değerinin bir değeri.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Workgroup değerini alır.

**Returns:**
int - Workgroup değerinin bir değeri.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Dahili kullanım için ayrılmıştır.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


[Resource](../../com.aspose.tasks/resource) sınıfının örneği için bir hash kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


IsBudget ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


IsCostResource ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


IsEnterprise ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


IsGeneric ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


IsNull ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Kaynağın kök kaynak olup olmadığını gösteren bayrağı alır. Kök kaynak, MS Project formatlarının iç işleyişini desteklemek için tasarlanmış özel bir kaynaktır ve kullanıcının kodundan doğrudan kullanılmak üzere tasarlanmamıştır.

**Returns:**
boolean - kaynağın kök kaynak olup olmadığını gösteren bayrak.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


IsTeamAssignmentPool ayarlı olup olmadığını gösteren değeri alır.

**Returns:**
boolean - IsTeamAssignmentPool'un ayarlanıp ayarlanmadığını gösteren bir değer.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Belirtilen özelliği bu konteynerde belirtilen değere eşler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | belirtilen özellik anahtarı. Özellik anahtarını almak için [Rsc](../../com.aspose.tasks/rsc). |
| değer. | java.util.Date | değer. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | ACWP değerinin bir değeri. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


AccrueAt değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | AccrueAt değerinin bir değeri. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


ActiveDirectoryGuid değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | ActiveDirectoryGuid değerinin bir değeri. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | ActualCost değerinin bir değeri. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | ActualOvertimeCost değerinin bir değeri. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork değerinin bir değeri. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected değerinin bir değeri. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork değerinin bir değeri. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected değerinin bir değeri. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | AssignmentOwner değerinin bir değeri. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | AssignmentOwnerGuid değerinin bir değeri. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


AvailableFrom değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | AvailableFrom'ın bir değeri. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


AvailableTo değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | AvailableTo'nun bir değeri. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | BCWP'nin bir değeri. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | BCWS'nin bir değeri. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | BookingType'ın bir değeri. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


IsBudget'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsBudget'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | BudgetCost'in bir değeri. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork'un bir değeri. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | CV'nin bir değeri. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Calendar'ın değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | Calendar'ın bir değeri. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


CanLevel'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | CanLevel'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Code'un değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Code'un bir değeri. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost'un değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | Cost'un bir değeri. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


CostCenter'ın değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | CostCenter'ın bir değeri. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


CostPerUse'un değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | CostPerUse'ın bir değeri. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


IsCostResource'un ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsCostResource'un ayarlanıp ayarlanmadığını gösteren bir değer. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance'ın değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | CostVariance'ın bir değeri. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created'ın değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Created'ın bir değeri. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


EMailAddress'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | EMailAddress'in bir değeri. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


IsEnterprise'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsEnterprise'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Finish'ın bir değeri. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


IsGeneric'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsGeneric'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Group'un değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Group'un bir değeri. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Guid'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Guid'in bir değeri. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Bir kaynakla ilişkili bir köprünün başlığını veya açıklayıcı metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | bir kaynakla ilişkili bir hyperlink'in başlığı veya açıklayıcı metni. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Bir kaynakla ilişkili bir köprünün adresini ayarlar.

--------------------

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | kaynakla ilişkili bir köprü için adres. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Bir kaynakla ilişkili bir köprünün bir belgedeki belirli konumunu ayarlar.

--------------------

Köprünün tam adresi (Microsoft Project'teki Hyperlink Href), HyperlinkAddress ve HyperlinkSubAddress'in birleştirilmesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | kaynakla ilişkili bir köprüdeki belgede belirli konum. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Id'nin değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Id değeri. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Inactive'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Inactive'in ayarlanıp ayarlanmadığını gösteren değer. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Initials'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Initials değeri. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


MaterialLabel'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | MaterialLabel değeri. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


MaxUnits'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | MaxUnits değeri. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Name'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Name değeri. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


NotesRTF'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | NotesRTF değeri. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


NotesText'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | NotesText değeri. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


IsNull'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | IsNull'in ayarlanıp ayarlanmadığını gösteren değer. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Overallocated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | Overallocated'in ayarlanıp ayarlanmadığını gösteren değer. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | OvertimeCost değeri. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


OvertimeRate'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | OvertimeRate değeri. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


OvertimeRateFormat'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | OvertimeRateFormat değeri. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork değeri. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | PeakUnits değeri. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | PercentWorkComplete değeri. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Phonetics'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Phonetics değeri. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork değeri. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | RemainingCost değeri. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | RemainingOvertimeCost değeri. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork değeri. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork değeri. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | SV değeri. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


StandardRate'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | StandardRate'in bir değeri. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


StandardRateFormat'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | StandardRateFormat'in bir değeri. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Start'ın bir değeri. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


IsTeamAssignmentPool'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | IsTeamAssignmentPool'un ayarlanıp ayarlanmadığını gösteren bir değer. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneğini ayarlar.

--------------------

Okuma yalnızca XML formatı için desteklenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | Bu nesne için [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneği. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Type değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Type'ın bir değeri. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Uid'nin bir değeri. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


WindowsUserAccount değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | WindowsUserAccount'un bir değeri. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work'in bir değeri. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


WorkVariance değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | WorkVariance'ın bir değeri. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Workgroup değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Workgroup'un bir değeri. |

### toString() {#toString--}
```
public String toString()
```


Bu, [Resource](../../com.aspose.tasks/resource) sınıfının örneğinin kısa dize temsiliini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişebilir.

**Returns:**
java.lang.String - kaynak nesneyi temsil eden kısa dize.

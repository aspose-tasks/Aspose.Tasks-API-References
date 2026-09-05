---
title: "Resource"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili sumber daya dalam sebuah proyek."
type: docs
weight: 248
url: /id/java/com.aspose.tasks/resource/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class Resource extends IContainer<Byte> implements System.IEquatable<Resource>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Mewakili sumber daya dalam sebuah proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [canLevel()](#canLevel--) | Mendapatkan nilai yang menunjukkan apakah CanLevel diatur atau tidak. |
| [delete()](#delete--) | Menghapus sumber daya dan penugasannya dari proyek. |
| [equals(Resource other)](#equals-com.aspose.tasks.Resource-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [Resource](../../com.aspose.tasks/resource). |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getACWP()](#getACWP--) | Memperoleh nilai ACWP. |
| [getAccrueAt()](#getAccrueAt--) | Memperoleh nilai AccrueAt. |
| [getActiveDirectoryGuid()](#getActiveDirectoryGuid--) | Memperoleh nilai ActiveDirectoryGuid. |
| [getActualCost()](#getActualCost--) | Memperoleh nilai ActualCost. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Memperoleh nilai ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Memperoleh nilai ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Memperoleh nilai ActualOvertimeWorkProtected. |
| [getActualWork()](#getActualWork--) | Memperoleh nilai ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Memperoleh nilai ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Memperoleh nilai AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Memperoleh nilai AssignmentOwnerGuid. |
| [getAssignments()](#getAssignments--) | Memperoleh koleksi penugasan sumber daya untuk objek ini. |
| [getAvailabilityPeriods()](#getAvailabilityPeriods--) | Memperoleh instance dari kelas [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). |
| [getAvailableFrom()](#getAvailableFrom--) | Memperoleh nilai AvailableFrom. |
| [getAvailableTo()](#getAvailableTo--) | Memperoleh nilai AvailableTo. |
| [getBCWP()](#getBCWP--) | Memperoleh nilai BCWP. |
| [getBCWS()](#getBCWS--) | Memperoleh nilai BCWS. |
| [getBaselines()](#getBaselines--) | Memperoleh instance BaselineCollection untuk objek ini. |
| [getBookingType()](#getBookingType--) | Memperoleh nilai BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Memperoleh nilai BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Memperoleh nilai BudgetWork. |
| [getCV()](#getCV--) | Memperoleh nilai CV. |
| [getCalendar()](#getCalendar--) | Memperoleh nilai Calendar. |
| [getCode()](#getCode--) | Mendapatkan nilai Code. |
| [getCost()](#getCost--) | Mendapatkan nilai Cost. |
| [getCostCenter()](#getCostCenter--) | Mendapatkan nilai CostCenter. |
| [getCostPerUse()](#getCostPerUse--) | Mendapatkan nilai CostPerUse. |
| [getCostVariance()](#getCostVariance--) | Mendapatkan nilai CostVariance. |
| [getCreated()](#getCreated--) | Mendapatkan nilai Created. |
| [getEMailAddress()](#getEMailAddress--) | Mendapatkan nilai EMailAddress. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Mendapatkan nilai-nilai atribut yang diperluas. |
| [getFinish()](#getFinish--) | Mendapatkan nilai Finish. |
| [getGroup()](#getGroup--) | Mendapatkan nilai Group. |
| [getGuid()](#getGuid--) | Mendapatkan nilai Guid. |
| [getHyperlink()](#getHyperlink--) | Mendapatkan judul atau teks penjelasan dari hyperlink yang terkait dengan sumber daya. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Mendapatkan alamat untuk hyperlink yang terkait dengan sumber daya. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Mendapatkan lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan sumber daya. |
| [getId()](#getId--) | Mendapatkan nilai Id. |
| [getInactive()](#getInactive--) | Mendapatkan nilai yang menunjukkan apakah Inactive diatur atau tidak. |
| [getInitials()](#getInitials--) | Mendapatkan nilai Initials. |
| [getItems()](#getItems--) | Mendapatkan sumber daya anak. |
| [getMaterialLabel()](#getMaterialLabel--) | Mendapatkan nilai MaterialLabel. |
| [getMaxUnits()](#getMaxUnits--) | Mendapatkan nilai MaxUnits. |
| [getName()](#getName--) | Mendapatkan nilai Name. |
| [getNotesRTF()](#getNotesRTF--) | Mendapatkan nilai NotesRTF. |
| [getNotesText()](#getNotesText--) | Mendapatkan nilai NotesText. |
| [getOutlineCode()](#getOutlineCode--) | Mendapatkan objek OutlineCodeCollection. |
| [getOverallocated()](#getOverallocated--) | Mendapatkan nilai yang menunjukkan apakah Overallocated diatur atau tidak. |
| [getOvertimeCost()](#getOvertimeCost--) | Mendapatkan nilai OvertimeCost. |
| [getOvertimeRate()](#getOvertimeRate--) | Mendapatkan nilai OvertimeRate. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Mendapatkan nilai OvertimeRateFormat. |
| [getOvertimeWork()](#getOvertimeWork--) | Mendapatkan nilai OvertimeWork. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk untuk kontainer ini. |
| [getPeakUnits()](#getPeakUnits--) | Mendapatkan nilai PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Mendapatkan nilai PercentWorkComplete. |
| [getPhonetics()](#getPhonetics--) | Mendapatkan nilai Phonetics. |
| [getRates()](#getRates--) | Mendapatkan instance dari kelas [RateCollection](../../com.aspose.tasks/ratecollection) untuk objek ini. |
| [getRegularWork()](#getRegularWork--) | Mendapatkan nilai RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Mendapatkan nilai RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Mendapatkan nilai RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Mendapatkan nilai RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Mendapatkan nilai RemainingWork. |
| [getSV()](#getSV--) | Mendapatkan nilai SV. |
| [getStandardRate()](#getStandardRate--) | Mendapatkan nilai StandardRate. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Mendapatkan nilai StandardRateFormat. |
| [getStart()](#getStart--) | Mendapatkan nilai Start. |
| [getTimephasedData()](#getTimephasedData--) | Mendapatkan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Mengembalikan [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini dengan nilai `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dalam rentang tanggal mulai dan akhir yang diberikan. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Mengembalikan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini dengan nilai `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dalam rentang tanggal mulai dan akhir yang diberikan untuk [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) yang ditentukan. |
| [getType()](#getType--) | Mendapatkan nilai Type. |
| [getUid()](#getUid--) | Mendapatkan nilai Uid. |
| [getWindowsUserAccount()](#getWindowsUserAccount--) | Mendapatkan nilai WindowsUserAccount. |
| [getWork()](#getWork--) | Mendapatkan nilai Work. |
| [getWorkVariance()](#getWorkVariance--) | Mendapatkan nilai WorkVariance. |
| [getWorkgroup()](#getWorkgroup--) | Mendapatkan nilai Workgroup. |
| [hasChildren()](#hasChildren--) | \{@inheritDoc\} |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [Resource](../../com.aspose.tasks/resource). |
| [isBudget()](#isBudget--) | Mendapatkan nilai yang menunjukkan apakah IsBudget diatur atau tidak. |
| [isCostResource()](#isCostResource--) | Mendapatkan nilai yang menunjukkan apakah IsCostResource diatur atau tidak. |
| [isEnterprise()](#isEnterprise--) | Mendapatkan nilai yang menunjukkan apakah IsEnterprise diatur atau tidak. |
| [isGeneric()](#isGeneric--) | Mendapatkan nilai yang menunjukkan apakah IsGeneric diatur atau tidak. |
| [isNull()](#isNull--) | Mendapatkan nilai yang menunjukkan apakah IsNull diatur atau tidak. |
| [isRoot()](#isRoot--) | Mendapatkan flag yang menunjukkan apakah resource adalah resource akar. |
| [isTeamAssignmentPool()](#isTeamAssignmentPool--) | Mendapatkan nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak. |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [setACWP(double value)](#setACWP-double-) | Mengatur nilai ACWP. |
| [setAccrueAt(int value)](#setAccrueAt-int-) | Mengatur nilai AccrueAt. |
| [setActiveDirectoryGuid(String value)](#setActiveDirectoryGuid-java.lang.String-) | Mengatur nilai ActiveDirectoryGuid. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Mengatur nilai ActualCost. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Mengatur nilai ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Mengatur nilai ActualOvertimeWorkProtected. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Mengatur nilai ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Mengatur nilai ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Mengatur nilai AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Mengatur nilai AssignmentOwnerGuid. |
| [setAvailableFrom(Date value)](#setAvailableFrom-java.util.Date-) | Mengatur nilai AvailableFrom. |
| [setAvailableTo(Date value)](#setAvailableTo-java.util.Date-) | Mengatur nilai AvailableTo. |
| [setBCWP(double value)](#setBCWP-double-) | Mengatur nilai BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Mengatur nilai BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Mengatur nilai BookingType. |
| [setBudget(NullableBool value)](#setBudget-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah IsBudget diatur atau tidak. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Mengatur nilai BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Mengatur nilai BudgetWork. |
| [setCV(double value)](#setCV-double-) | Mengatur nilai CV. |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | Mengatur nilai Calendar. |
| [setCanLevel(NullableBool value)](#setCanLevel-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah CanLevel diatur atau tidak. |
| [setCode(String value)](#setCode-java.lang.String-) | Mengatur nilai Code. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Mengatur nilai Cost. |
| [setCostCenter(String value)](#setCostCenter-java.lang.String-) | Mengatur nilai CostCenter. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Mengatur nilai CostPerUse. |
| [setCostResource(NullableBool value)](#setCostResource-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah IsCostResource diatur atau tidak. |
| [setCostVariance(double value)](#setCostVariance-double-) | Mengatur nilai CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Mengatur nilai Created. |
| [setEMailAddress(String value)](#setEMailAddress-java.lang.String-) | Mengatur nilai EMailAddress. |
| [setEnterprise(NullableBool value)](#setEnterprise-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah IsEnterprise diatur atau tidak. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Mengatur nilai Finish. |
| [setGeneric(NullableBool value)](#setGeneric-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah IsGeneric diatur atau tidak. |
| [setGroup(String value)](#setGroup-java.lang.String-) | Mengatur nilai Group. |
| [setGuid(String value)](#setGuid-java.lang.String-) | Mengatur nilai Guid. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Mengatur judul atau teks penjelas dari hyperlink yang terkait dengan sumber daya. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Mengatur alamat untuk hyperlink yang terkait dengan sumber daya. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Mengatur lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan sumber daya. |
| [setId(int value)](#setId-int-) | Mengatur nilai Id. |
| [setInactive(NullableBool value)](#setInactive-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah Inactive diatur atau tidak. |
| [setInitials(String value)](#setInitials-java.lang.String-) | Mengatur nilai Initials. |
| [setMaterialLabel(String value)](#setMaterialLabel-java.lang.String-) | Mengatur nilai MaterialLabel. |
| [setMaxUnits(double value)](#setMaxUnits-double-) | Mengatur nilai MaxUnits. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nilai Name. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Mengatur nilai NotesRTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Mengatur nilai NotesText. |
| [setNull(NullableBool value)](#setNull-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah IsNull diatur atau tidak. |
| [setOverallocated(NullableBool value)](#setOverallocated-com.aspose.tasks.NullableBool-) | Mengatur nilai yang menunjukkan apakah Overallocated diatur atau tidak. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Mengatur nilai OvertimeCost. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Mengatur nilai OvertimeRate. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Mengatur nilai OvertimeRateFormat. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Mengatur nilai PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Mengatur nilai PercentWorkComplete. |
| [setPhonetics(String value)](#setPhonetics-java.lang.String-) | Mengatur nilai Phonetics. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Mengatur nilai RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Mengatur nilai RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Mengatur nilai RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Mengatur nilai RemainingWork. |
| [setSV(double value)](#setSV-double-) | Mengatur nilai SV. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Mengatur nilai StandardRate. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Mengatur nilai StandardRateFormat. |
| [setStart(Date value)](#setStart-java.util.Date-) | Mengatur nilai Start. |
| [setTeamAssignmentPool(boolean value)](#setTeamAssignmentPool-boolean-) | Mengatur nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Mengatur sebuah instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |
| [setType(int value)](#setType-int-) | Mengatur nilai dari Type. |
| [setUid(int value)](#setUid-int-) | Mengatur nilai dari Uid. |
| [setWindowsUserAccount(String value)](#setWindowsUserAccount-java.lang.String-) | Mengatur nilai dari WindowsUserAccount. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Mengatur nilai dari Work. |
| [setWorkVariance(double value)](#setWorkVariance-double-) | Mengatur nilai dari WorkVariance. |
| [setWorkgroup(int value)](#setWorkgroup-int-) | Mengatur nilai dari Workgroup. |
| [toString()](#toString--) | Mengembalikan representasi string singkat dari instance kelas [Resource](../../com.aspose.tasks/resource). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Rsc](../../com.aspose.tasks/rsc) untuk mendapatkan kunci properti. |

**Returns:**
T - nilai yang dipetakan ke properti ini dalam kontainer ini.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public void <T>set(Key<T,Byte> key, T val)
```


Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Rsc](../../com.aspose.tasks/rsc) untuk mendapatkan kunci properti. |
| val | T | nilai. |

### canLevel() {#canLevel--}
```
public final NullableBool canLevel()
```


Mendapatkan nilai yang menunjukkan apakah CanLevel diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether CanLevel is set or not.
### delete() {#delete--}
```
public final void delete()
```


Menghapus sumber daya dan penugasannya dari proyek.

### equals(Resource other) {#equals-com.aspose.tasks.Resource-}
```
public final boolean equals(Resource other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [Resource](../../com.aspose.tasks/resource).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [Resource](../../com.aspose.tasks/resource) | Instance kelas [Resource](../../com.aspose.tasks/resource) yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika instance [Resource](../../com.aspose.tasks/resource) yang ditentukan memiliki nilai Uid yang sama dengan instance ini; jika tidak, **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika objek yang ditentukan adalah Resource yang memiliki nilai Uid yang sama dengan instance ini; jika tidak, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Memperoleh nilai ACWP.

**Returns:**
double - nilai ACWP.
### getAccrueAt() {#getAccrueAt--}
```
public final int getAccrueAt()
```


Memperoleh nilai AccrueAt.

**Returns:**
int - nilai AccrueAt.
### getActiveDirectoryGuid() {#getActiveDirectoryGuid--}
```
public final String getActiveDirectoryGuid()
```


Memperoleh nilai ActiveDirectoryGuid.

**Returns:**
java.lang.String - nilai ActiveDirectoryGuid.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Memperoleh nilai ActualCost.

**Returns:**
java.math.BigDecimal - nilai ActualCost.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


Memperoleh nilai ActualOvertimeCost.

**Returns:**
java.math.BigDecimal - nilai ActualOvertimeCost.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


Memperoleh nilai ActualOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


Memperoleh nilai ActualOvertimeWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


Memperoleh nilai ActualWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


Memperoleh nilai ActualWorkProtected.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


Memperoleh nilai AssignmentOwner.

**Returns:**
java.lang.String - nilai AssignmentOwner.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


Memperoleh nilai AssignmentOwnerGuid.

**Returns:**
java.lang.String - nilai AssignmentOwnerGuid.
### getAssignments() {#getAssignments--}
```
public final ResourceAssignmentCollection getAssignments()
```


Memperoleh koleksi penugasan sumber daya untuk objek ini.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - a collection of resource assignments for this object.
### getAvailabilityPeriods() {#getAvailabilityPeriods--}
```
public final AvailabilityPeriodCollection getAvailabilityPeriods()
```


Mendapatkan instance dari kelas [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection). Kumpulan periode di mana sebuah sumber daya tersedia.

**Returns:**
[AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) - a the instance of the [AvailabilityPeriodCollection](../../com.aspose.tasks/availabilityperiodcollection) class.
### getAvailableFrom() {#getAvailableFrom--}
```
public final Date getAvailableFrom()
```


Memperoleh nilai AvailableFrom.

**Returns:**
java.util.Date - sebuah nilai dari AvailableFrom.
### getAvailableTo() {#getAvailableTo--}
```
public final Date getAvailableTo()
```


Memperoleh nilai AvailableTo.

**Returns:**
java.util.Date - sebuah nilai dari AvailableTo.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


Memperoleh nilai BCWP.

**Returns:**
double - sebuah nilai dari BCWP.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


Memperoleh nilai BCWS.

**Returns:**
double - sebuah nilai dari BCWS.
### getBaselines() {#getBaselines--}
```
public final BaselineCollection getBaselines()
```


Mendapatkan instance BaselineCollection untuk objek ini. Nilai baseline untuk sebuah sumber daya.

**Returns:**
[BaselineCollection](../../com.aspose.tasks/baselinecollection) - a BaselineCollection instance for this object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


Memperoleh nilai BookingType.

**Returns:**
int - sebuah nilai dari BookingType.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


Memperoleh nilai BudgetCost.

**Returns:**
java.math.BigDecimal - sebuah nilai dari BudgetCost.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


Memperoleh nilai BudgetWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


Memperoleh nilai CV.

**Returns:**
double - sebuah nilai dari CV.
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


Memperoleh nilai Calendar.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCode() {#getCode--}
```
public final String getCode()
```


Mendapatkan nilai Code.

**Returns:**
java.lang.String - sebuah nilai dari Code.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Mendapatkan nilai Cost.

**Returns:**
java.math.BigDecimal - sebuah nilai dari Cost.
### getCostCenter() {#getCostCenter--}
```
public final String getCostCenter()
```


Mendapatkan nilai CostCenter.

**Returns:**
java.lang.String - sebuah nilai dari CostCenter.
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Mendapatkan nilai CostPerUse.

**Returns:**
java.math.BigDecimal - sebuah nilai dari CostPerUse.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


Mendapatkan nilai CostVariance.

**Returns:**
double - sebuah nilai dari CostVariance.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Mendapatkan nilai Created.

**Returns:**
java.util.Date - sebuah nilai dari Created.
### getEMailAddress() {#getEMailAddress--}
```
public final String getEMailAddress()
```


Mendapatkan nilai EMailAddress.

**Returns:**
java.lang.String - sebuah nilai dari EMailAddress.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Mendapatkan nilai-nilai atribut yang diperluas.

--------------------

Dua potongan data diperlukan - sebuah penunjuk kembali ke tabel atribut yang diperluas yang ditentukan baik oleh unique ID atau Field ID, dan nilai yang ditentukan baik dengan nilai, atau sebuah penunjuk kembali ke daftar nilai.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - the values of an extended attribute.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Mendapatkan nilai Finish.

**Returns:**
java.util.Date - sebuah nilai dari Finish.
### getGroup() {#getGroup--}
```
public final String getGroup()
```


Mendapatkan nilai Group.

**Returns:**
java.lang.String - sebuah nilai dari Group.
### getGuid() {#getGuid--}
```
public final String getGuid()
```


Mendapatkan nilai Guid.

**Returns:**
java.lang.String - sebuah nilai dari Guid.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Mendapatkan judul atau teks penjelasan dari hyperlink yang terkait dengan sumber daya.

**Returns:**
java.lang.String - judul atau teks penjelas dari hyperlink yang terkait dengan sebuah sumber daya.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Mendapatkan alamat untuk hyperlink yang terkait dengan sumber daya.

--------------------

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

**Returns:**
java.lang.String - alamat untuk hyperlink yang terkait dengan sebuah sumber daya.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Mendapatkan lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan sumber daya.

--------------------

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

**Returns:**
java.lang.String - lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan sebuah sumber daya.
### getId() {#getId--}
```
public final int getId()
```


Mendapatkan nilai Id.

**Returns:**
int - sebuah nilai dari Id.
### getInactive() {#getInactive--}
```
public final NullableBool getInactive()
```


Mendapatkan nilai yang menunjukkan apakah Inactive diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Inactive is set or not.
### getInitials() {#getInitials--}
```
public final String getInitials()
```


Mendapatkan nilai Initials.

**Returns:**
java.lang.String - sebuah nilai dari Initials.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Mendapatkan sumber daya anak.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - sumber daya anak.
### getMaterialLabel() {#getMaterialLabel--}
```
public final String getMaterialLabel()
```


Mendapatkan nilai MaterialLabel.

**Returns:**
java.lang.String - sebuah nilai MaterialLabel.
### getMaxUnits() {#getMaxUnits--}
```
public final double getMaxUnits()
```


Mendapatkan nilai MaxUnits.

**Returns:**
double - sebuah nilai MaxUnits.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nilai Name.

**Returns:**
java.lang.String - sebuah nilai Name.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Mendapatkan nilai NotesRTF.

**Returns:**
java.lang.String - sebuah nilai NotesRTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Mendapatkan nilai NotesText.

**Returns:**
java.lang.String - sebuah nilai NotesText.
### getOutlineCode() {#getOutlineCode--}
```
public final OutlineCodeCollection getOutlineCode()
```


Mendapatkan objek OutlineCodeCollection. Nilai dari kode outline.

--------------------

Dua potongan data diperlukan - sebuah pointer ke tabel kode outline yang ditentukan oleh FieldID, dan nilai yang ditentukan baik oleh pointer ValueID atau ValueGUID ke daftar nilai.

**Returns:**
[OutlineCodeCollection](../../com.aspose.tasks/outlinecodecollection) - an OutlineCodeCollection object.
### getOverallocated() {#getOverallocated--}
```
public final NullableBool getOverallocated()
```


Mendapatkan nilai yang menunjukkan apakah Overallocated diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Overallocated is set or not.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Mendapatkan nilai OvertimeCost.

**Returns:**
java.math.BigDecimal - sebuah nilai OvertimeCost.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Mendapatkan nilai OvertimeRate.

**Returns:**
java.math.BigDecimal - sebuah nilai OvertimeRate.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Mendapatkan nilai OvertimeRateFormat.

**Returns:**
int - sebuah nilai OvertimeRateFormat.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


Mendapatkan nilai OvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan proyek induk untuk kontainer ini.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this container.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


Mendapatkan nilai PeakUnits.

**Returns:**
double - sebuah nilai PeakUnits.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


Mendapatkan nilai PercentWorkComplete.

**Returns:**
int - sebuah nilai PercentWorkComplete.
### getPhonetics() {#getPhonetics--}
```
public final String getPhonetics()
```


Mendapatkan nilai Phonetics.

**Returns:**
java.lang.String - sebuah nilai Phonetics.
### getRates() {#getRates--}
```
public final RateCollection getRates()
```


Mendapatkan instance dari kelas [RateCollection](../../com.aspose.tasks/ratecollection) untuk objek ini. Kumpulan periode dan tarif yang terkait dengan masing-masing.

**Returns:**
[RateCollection](../../com.aspose.tasks/ratecollection) - a the instance of the [RateCollection](../../com.aspose.tasks/ratecollection) class for this object.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


Mendapatkan nilai RegularWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


Mendapatkan nilai RemainingCost.

**Returns:**
java.math.BigDecimal - sebuah nilai RemainingCost.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


Mendapatkan nilai RemainingOvertimeCost.

**Returns:**
java.math.BigDecimal - sebuah nilai RemainingOvertimeCost.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


Mendapatkan nilai RemainingOvertimeWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


Mendapatkan nilai RemainingWork.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getSV() {#getSV--}
```
public final double getSV()
```


Mendapatkan nilai SV.

**Returns:**
double - sebuah nilai SV.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Mendapatkan nilai StandardRate.

**Returns:**
java.math.BigDecimal - sebuah nilai StandardRate.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Mendapatkan nilai StandardRateFormat.

**Returns:**
int - sebuah nilai StandardRateFormat.
### getStart() {#getStart--}
```
public final Date getStart()
```


Mendapatkan nilai Start.

**Returns:**
java.util.Date - sebuah nilai Start.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Mendapatkan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini.

--------------------

Membaca didukung hanya untuk format XML.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - an instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class for this object.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Mengembalikan [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini dengan nilai `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dalam rentang tanggal mulai dan akhir yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai untuk data timephased. |
| akhir | java.util.Date | Tanggal akhir untuk data berwaktu. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of [TimephasedData](../../com.aspose.tasks/timephaseddata).
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Mengembalikan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini dengan nilai `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)) dalam rentang tanggal mulai dan akhir yang diberikan untuk [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai untuk data berwaktu. |
| akhir | java.util.Date | Tanggal akhir untuk data berwaktu. |
| timephasedType | byte | Tipe data berwaktu ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - List of `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resource\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resource\#setTimephasedData-TimephasedDataCollection-)).
### getType() {#getType--}
```
public final int getType()
```


Mendapatkan nilai Type.

**Returns:**
int - nilai dari Type.
### getUid() {#getUid--}
```
public final int getUid()
```


Mendapatkan nilai Uid.

**Returns:**
int - nilai dari Uid.
### getWindowsUserAccount() {#getWindowsUserAccount--}
```
public final String getWindowsUserAccount()
```


Mendapatkan nilai WindowsUserAccount.

**Returns:**
java.lang.String - nilai dari WindowsUserAccount.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Mendapatkan nilai Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkVariance() {#getWorkVariance--}
```
public final double getWorkVariance()
```


Mendapatkan nilai WorkVariance.

**Returns:**
double - nilai dari WorkVariance.
### getWorkgroup() {#getWorkgroup--}
```
public final int getWorkgroup()
```


Mendapatkan nilai Workgroup.

**Returns:**
int - nilai dari Workgroup.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Dicadangkan untuk penggunaan internal.

**Returns:**
boolean - \{@inheritDoc\}
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [Resource](../../com.aspose.tasks/resource).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### isBudget() {#isBudget--}
```
public final NullableBool isBudget()
```


Mendapatkan nilai yang menunjukkan apakah IsBudget diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsBudget is set or not.
### isCostResource() {#isCostResource--}
```
public final NullableBool isCostResource()
```


Mendapatkan nilai yang menunjukkan apakah IsCostResource diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsCostResource is set or not.
### isEnterprise() {#isEnterprise--}
```
public final NullableBool isEnterprise()
```


Mendapatkan nilai yang menunjukkan apakah IsEnterprise diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsEnterprise is set or not.
### isGeneric() {#isGeneric--}
```
public final NullableBool isGeneric()
```


Mendapatkan nilai yang menunjukkan apakah IsGeneric diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsGeneric is set or not.
### isNull() {#isNull--}
```
public final NullableBool isNull()
```


Mendapatkan nilai yang menunjukkan apakah IsNull diatur atau tidak.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether IsNull is set or not.
### isRoot() {#isRoot--}
```
public boolean isRoot()
```


Mendapatkan flag yang menunjukkan apakah sumber daya adalah sumber daya akar. Sumber daya akar adalah sumber daya khusus yang dimaksudkan untuk mendukung internal format MS Project dan tidak dimaksudkan untuk digunakan langsung dari kode pengguna.

**Returns:**
boolean - flag yang menunjukkan apakah sumber daya adalah sumber daya akar.
### isTeamAssignmentPool() {#isTeamAssignmentPool--}
```
public final boolean isTeamAssignmentPool()
```


Mendapatkan nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak.

**Returns:**
boolean - nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak.
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | kunci properti yang ditentukan. [Rsc](../../com.aspose.tasks/rsc) untuk mendapatkan kunci properti. |
| val | java.util.Date | nilai. |

### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Mengatur nilai ACWP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari ACWP. |

### setAccrueAt(int value) {#setAccrueAt-int-}
```
public final void setAccrueAt(int value)
```


Mengatur nilai AccrueAt.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari AccrueAt. |

### setActiveDirectoryGuid(String value) {#setActiveDirectoryGuid-java.lang.String-}
```
public final void setActiveDirectoryGuid(String value)
```


Mengatur nilai ActiveDirectoryGuid.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari ActiveDirectoryGuid. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Mengatur nilai ActualCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari ActualCost. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


Mengatur nilai ActualOvertimeCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari ActualOvertimeCost. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


Mengatur nilai ActualOvertimeWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari ActualOvertimeWork. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


Mengatur nilai ActualOvertimeWorkProtected.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari ActualOvertimeWorkProtected. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


Mengatur nilai ActualWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari ActualWork. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


Mengatur nilai ActualWorkProtected.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari ActualWorkProtected. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


Mengatur nilai AssignmentOwner.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari AssignmentOwner. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


Mengatur nilai AssignmentOwnerGuid.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari AssignmentOwnerGuid. |

### setAvailableFrom(Date value) {#setAvailableFrom-java.util.Date-}
```
public final void setAvailableFrom(Date value)
```


Mengatur nilai AvailableFrom.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari AvailableFrom. |

### setAvailableTo(Date value) {#setAvailableTo-java.util.Date-}
```
public final void setAvailableTo(Date value)
```


Mengatur nilai AvailableTo.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari AvailableTo. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


Mengatur nilai BCWP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari BCWP. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


Mengatur nilai BCWS.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari BCWS. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


Mengatur nilai BookingType.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari BookingType. |

### setBudget(NullableBool value) {#setBudget-com.aspose.tasks.NullableBool-}
```
public final void setBudget(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah IsBudget diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah IsBudget diatur atau tidak. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


Mengatur nilai BudgetCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari BudgetCost. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


Mengatur nilai BudgetWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari BudgetWork. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


Mengatur nilai CV.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari CV. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Mengatur nilai Calendar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | nilai dari Calendar. |

### setCanLevel(NullableBool value) {#setCanLevel-com.aspose.tasks.NullableBool-}
```
public final void setCanLevel(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah CanLevel diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah CanLevel diatur atau tidak. |

### setCode(String value) {#setCode-java.lang.String-}
```
public final void setCode(String value)
```


Mengatur nilai Code.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari Code. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Mengatur nilai Cost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari Cost. |

### setCostCenter(String value) {#setCostCenter-java.lang.String-}
```
public final void setCostCenter(String value)
```


Mengatur nilai CostCenter.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari CostCenter. |

### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Mengatur nilai CostPerUse.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari CostPerUse. |

### setCostResource(NullableBool value) {#setCostResource-com.aspose.tasks.NullableBool-}
```
public final void setCostResource(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah IsCostResource diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah IsCostResource diatur atau tidak. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


Mengatur nilai CostVariance.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari CostVariance. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Mengatur nilai Created.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Created. |

### setEMailAddress(String value) {#setEMailAddress-java.lang.String-}
```
public final void setEMailAddress(String value)
```


Mengatur nilai EMailAddress.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari EMailAddress. |

### setEnterprise(NullableBool value) {#setEnterprise-com.aspose.tasks.NullableBool-}
```
public final void setEnterprise(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah IsEnterprise diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah IsEnterprise diatur atau tidak. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Mengatur nilai Finish.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Finish. |

### setGeneric(NullableBool value) {#setGeneric-com.aspose.tasks.NullableBool-}
```
public final void setGeneric(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah IsGeneric diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah IsGeneric diatur atau tidak. |

### setGroup(String value) {#setGroup-java.lang.String-}
```
public final void setGroup(String value)
```


Mengatur nilai Group.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari Group. |

### setGuid(String value) {#setGuid-java.lang.String-}
```
public final void setGuid(String value)
```


Mengatur nilai Guid.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari Guid. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Mengatur judul atau teks penjelas dari hyperlink yang terkait dengan sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | judul atau teks penjelasan dari hyperlink yang terkait dengan sumber daya. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Mengatur alamat untuk hyperlink yang terkait dengan sumber daya.

--------------------

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | alamat untuk tautan yang terkait dengan sumber daya. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Mengatur lokasi spesifik dalam dokumen pada hyperlink yang terkait dengan sumber daya.

--------------------

Alamat lengkap (Hyperlink Href dalam Microsoft Project) dari hyperlink adalah penggabungan HyperlinkAddress dan HyperlinkSubAddress.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | lokasi spesifik dalam dokumen pada tautan yang terkait dengan sumber daya. |

### setId(int value) {#setId-int-}
```
public final void setId(int value)
```


Mengatur nilai Id.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai Id. |

### setInactive(NullableBool value) {#setInactive-com.aspose.tasks.NullableBool-}
```
public final void setInactive(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah Inactive diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah Inactive diatur atau tidak. |

### setInitials(String value) {#setInitials-java.lang.String-}
```
public final void setInitials(String value)
```


Mengatur nilai Initials.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai Initials. |

### setMaterialLabel(String value) {#setMaterialLabel-java.lang.String-}
```
public final void setMaterialLabel(String value)
```


Mengatur nilai MaterialLabel.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai MaterialLabel. |

### setMaxUnits(double value) {#setMaxUnits-double-}
```
public final void setMaxUnits(double value)
```


Mengatur nilai MaxUnits.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai MaxUnits. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Mengatur nilai Name.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai Name. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Mengatur nilai NotesRTF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai NotesRTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Mengatur nilai NotesText.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai NotesText. |

### setNull(NullableBool value) {#setNull-com.aspose.tasks.NullableBool-}
```
public final void setNull(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah IsNull diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah IsNull diatur atau tidak. |

### setOverallocated(NullableBool value) {#setOverallocated-com.aspose.tasks.NullableBool-}
```
public final void setOverallocated(NullableBool value)
```


Mengatur nilai yang menunjukkan apakah Overallocated diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | nilai yang menunjukkan apakah Overallocated diatur atau tidak. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Mengatur nilai OvertimeCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai OvertimeCost. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Mengatur nilai OvertimeRate.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai OvertimeRate. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Mengatur nilai OvertimeRateFormat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai OvertimeRateFormat. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


Mengatur nilai OvertimeWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai OvertimeWork. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


Mengatur nilai PeakUnits.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai PeakUnits. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


Mengatur nilai PercentWorkComplete.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai PercentWorkComplete. |

### setPhonetics(String value) {#setPhonetics-java.lang.String-}
```
public final void setPhonetics(String value)
```


Mengatur nilai Phonetics.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai Phonetics. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


Mengatur nilai RegularWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai RegularWork. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


Mengatur nilai RemainingCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai RemainingCost. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


Mengatur nilai RemainingOvertimeCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai RemainingOvertimeCost. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


Mengatur nilai RemainingOvertimeWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai RemainingOvertimeWork. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


Mengatur nilai RemainingWork.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai RemainingWork. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Mengatur nilai SV.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai SV. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Mengatur nilai StandardRate.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari StandardRate. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Mengatur nilai StandardRateFormat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari StandardRateFormat. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Mengatur nilai Start.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Start. |

### setTeamAssignmentPool(boolean value) {#setTeamAssignmentPool-boolean-}
```
public final void setTeamAssignmentPool(boolean value)
```


Mengatur nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah IsTeamAssignmentPool diatur atau tidak. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Mengatur sebuah instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini.

--------------------

Membaca didukung hanya untuk format XML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) untuk objek ini. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Mengatur nilai dari Type.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari Type. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Mengatur nilai dari Uid.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari Uid. |

### setWindowsUserAccount(String value) {#setWindowsUserAccount-java.lang.String-}
```
public final void setWindowsUserAccount(String value)
```


Mengatur nilai dari WindowsUserAccount.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai dari WindowsUserAccount. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Mengatur nilai dari Work.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari Work. |

### setWorkVariance(double value) {#setWorkVariance-double-}
```
public final void setWorkVariance(double value)
```


Mengatur nilai dari WorkVariance.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari WorkVariance. |

### setWorkgroup(int value) {#setWorkgroup-int-}
```
public final void setWorkgroup(int value)
```


Mengatur nilai dari Workgroup.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari Workgroup. |

### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string pendek dari instance kelas [Resource](../../com.aspose.tasks/resource). Detail tepat dari representasi tersebut tidak ditentukan dan dapat berubah.

**Returns:**
java.lang.String - string pendek yang mewakili objek sumber daya.

---
title: "ResourceAssignment"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili penugasan sumber daya dalam sebuah proyek."
type: docs
weight: 249
url: /id/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Mewakili penugasan sumber daya dalam sebuah proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini. |
| [delete()](#delete--) | Menghapus penugasan sumber daya dari koleksi penugasan proyek. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getACWP()](#getACWP--) | Memperoleh nilai ACWP. |
| [getActualCost()](#getActualCost--) | Memperoleh nilai ActualCost. |
| [getActualFinish()](#getActualFinish--) | Mendapatkan nilai ActualFinish. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | Memperoleh nilai ActualOvertimeCost. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | Memperoleh nilai ActualOvertimeWork. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | Memperoleh nilai ActualOvertimeWorkProtected. |
| [getActualStart()](#getActualStart--) | Mendapatkan nilai ActualStart. |
| [getActualWork()](#getActualWork--) | Memperoleh nilai ActualWork. |
| [getActualWorkProtected()](#getActualWorkProtected--) | Memperoleh nilai ActualWorkProtected. |
| [getAssignmentOwner()](#getAssignmentOwner--) | Memperoleh nilai AssignmentOwner. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | Memperoleh nilai AssignmentOwnerGuid. |
| [getBCWP()](#getBCWP--) | Memperoleh nilai BCWP. |
| [getBCWS()](#getBCWS--) | Memperoleh nilai BCWS. |
| [getBaselines()](#getBaselines--) | Mendapatkan objek AssignmentBaselineCollection. |
| [getBookingType()](#getBookingType--) | Memperoleh nilai BookingType. |
| [getBudgetCost()](#getBudgetCost--) | Memperoleh nilai BudgetCost. |
| [getBudgetWork()](#getBudgetWork--) | Memperoleh nilai BudgetWork. |
| [getCV()](#getCV--) | Memperoleh nilai CV. |
| [getConfirmed()](#getConfirmed--) | Mendapatkan nilai yang menunjukkan apakah Confirmed diatur atau tidak. |
| [getCost()](#getCost--) | Mendapatkan nilai Cost. |
| [getCostRateTableType()](#getCostRateTableType--) | Mendapatkan nilai CostRateTableType. |
| [getCostVariance()](#getCostVariance--) | Mendapatkan nilai CostVariance. |
| [getCreated()](#getCreated--) | Mendapatkan nilai Created. |
| [getDelay()](#getDelay--) | Mendapatkan nilai Delay. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Mendapatkan instance dari kelas ExtendedAttributeCollection untuk objek ini. |
| [getFinish()](#getFinish--) | Mendapatkan nilai Finish. |
| [getFinishVariance()](#getFinishVariance--) | Mendapatkan nilai FinishVariance. |
| [getFixedMaterial()](#getFixedMaterial--) | Mendapatkan nilai yang menunjukkan apakah FixedMaterial diatur atau tidak. |
| [getGuid()](#getGuid--) | Mendapatkan pengidentifikasi unik untuk penugasan ini. |
| [getHyperlink()](#getHyperlink--) | Mendapatkan nilai Hyperlink. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | Mendapatkan nilai HyperlinkAddress. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | Mendapatkan nilai HyperlinkSubAddress. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | Mendapatkan nilai LevelingDelay. |
| [getLinkedFields()](#getLinkedFields--) | Mendapatkan nilai yang menunjukkan apakah LinkedFields diatur atau tidak. |
| [getMilestone()](#getMilestone--) | Mendapatkan nilai yang menunjukkan apakah Milestone diatur atau tidak. |
| [getNotesRTF()](#getNotesRTF--) | Mendapatkan catatan teks dalam format RTF. |
| [getNotesText()](#getNotesText--) | Mendapatkan teks polos catatan yang diekstrak dari data RTF. |
| [getOverallocated()](#getOverallocated--) | Mendapatkan nilai yang menunjukkan apakah Overallocated diatur atau tidak. |
| [getOvertimeCost()](#getOvertimeCost--) | Mendapatkan nilai OvertimeCost. |
| [getOvertimeWork()](#getOvertimeWork--) | Mendapatkan nilai OvertimeWork. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk untuk penugasan ini. |
| [getPeakUnits()](#getPeakUnits--) | Mendapatkan nilai PeakUnits. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | Mendapatkan nilai PercentWorkComplete. |
| [getRateScale()](#getRateScale--) | Mendapatkan nilai RateScale. |
| [getRegularWork()](#getRegularWork--) | Mendapatkan nilai RegularWork. |
| [getRemainingCost()](#getRemainingCost--) | Mendapatkan nilai RemainingCost. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | Mendapatkan nilai RemainingOvertimeCost. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | Mendapatkan nilai RemainingOvertimeWork. |
| [getRemainingWork()](#getRemainingWork--) | Mendapatkan nilai RemainingWork. |
| [getResource()](#getResource--) | Sumber daya yang ditugaskan ke tugas. |
| [getResponsePending()](#getResponsePending--) | Mendapatkan nilai yang menunjukkan apakah ResponsePending diatur atau tidak. |
| [getResume()](#getResume--) | Mendapatkan nilai Resume. |
| [getSV()](#getSV--) | Mendapatkan nilai SV. |
| [getStart()](#getStart--) | Mendapatkan nilai Start. |
| [getStartVariance()](#getStartVariance--) | Mendapatkan nilai StartVariance. |
| [getStop()](#getStop--) | Mendapatkan nilai Stop. |
| [getSummary()](#getSummary--) | Mendapatkan nilai yang menunjukkan apakah Summary diatur atau tidak. |
| [getTask()](#getTask--) | Tugas yang diberikan kepada sumber daya. |
| [getTimephasedData()](#getTimephasedData--) | Mendapatkan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi elemen `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) kelas. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Mengembalikan objek [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) dengan instance `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) kelas dalam tanggal mulai dan akhir yang diberikan dari [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork). |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Mengembalikan instance kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi instance `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) kelas dalam tanggal mulai dan akhir yang diberikan dari [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype). |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Mendapatkan jumlah kerja timephased untuk interval tanggal waktu yang ditentukan. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Mendapatkan jumlah kerja timephased untuk interval tanggal waktu yang ditentukan. |
| [getUid()](#getUid--) | Mendapatkan nilai Uid. |
| [getUnits()](#getUnits--) | Mendapatkan nilai Units. |
| [getUpdateNeeded()](#getUpdateNeeded--) | Mendapatkan nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak. |
| [getVAC()](#getVAC--) | Mendapatkan nilai VAC. |
| [getWork()](#getWork--) | Mendapatkan nilai Work. |
| [getWorkContour()](#getWorkContour--) | Mendapatkan nilai WorkContour. |
| [getWorkVariance()](#getWorkVariance--) | Mendapatkan nilai WorkVariance. |
| [hasChildren()](#hasChildren--) | Mendapatkan nilai yang menunjukkan bahwa penugasan sumber daya ini memiliki anak. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | Mendapatkan nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Menghasilkan daftar data berfase waktu. |
| [setACWP(double value)](#setACWP-double-) | Mengatur nilai ACWP. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | Mengatur nilai ActualCost. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | Mengatur nilai ActualFinish. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | Mengatur nilai ActualOvertimeCost. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai ActualOvertimeWork. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | Mengatur nilai ActualOvertimeWorkProtected. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | Mengatur nilai ActualStart. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | Mengatur nilai ActualWork. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | Mengatur nilai ActualWorkProtected. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | Mengatur nilai AssignmentOwner. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | Mengatur nilai AssignmentOwnerGuid. |
| [setBCWP(double value)](#setBCWP-double-) | Mengatur nilai BCWP. |
| [setBCWS(double value)](#setBCWS-double-) | Mengatur nilai BCWS. |
| [setBookingType(int value)](#setBookingType-int-) | Mengatur nilai BookingType. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | Mengatur nilai BudgetCost. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | Mengatur nilai BudgetWork. |
| [setCV(double value)](#setCV-double-) | Mengatur nilai CV. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Mengatur nilai yang menunjukkan apakah Confirmed diatur atau tidak. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Mengatur nilai Cost. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | Mengatur nilai CostRateTableType. |
| [setCostVariance(double value)](#setCostVariance-double-) | Mengatur nilai CostVariance. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Mengatur nilai Created. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Mengatur nilai Delay. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Mengatur sebuah instance kelas ExtendedAttributeCollection untuk objek ini. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Mengatur nilai Finish. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | Mengatur nilai FinishVariance. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | Mengatur nilai yang menunjukkan apakah FixedMaterial diatur atau tidak. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | Mengatur nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Mengatur pengidentifikasi unik untuk penugasan ini. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Mengatur nilai Hyperlink. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | Mengatur nilai HyperlinkAddress. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | Mengatur nilai HyperlinkSubAddress. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | Mengatur nilai LevelingDelay. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | Mengatur nilai yang menunjukkan apakah LinkedFields diatur atau tidak. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Mengatur satuan untuk penugasan sumber daya material dengan konsumsi material variabel. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Mengatur nilai yang menunjukkan apakah Milestone diatur atau tidak. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Mengatur catatan teks dalam format RTF. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | Mengatur teks polos catatan yang diekstrak dari data RTF. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Mengatur nilai yang menunjukkan apakah Overallocated diatur atau tidak. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | Mengatur nilai OvertimeCost. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai OvertimeWork. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | Mengatur nilai PeakUnits. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | Mengatur nilai PercentWorkComplete. |
| [setRateScale(int value)](#setRateScale-int-) | Mengatur nilai RateScale. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | Mengatur nilai RegularWork. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | Mengatur nilai RemainingCost. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | Mengatur nilai RemainingOvertimeCost. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | Mengatur nilai RemainingOvertimeWork. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | Mengatur nilai RemainingWork. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | Sumber daya yang ditugaskan ke tugas. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | Mengatur nilai yang menunjukkan apakah ResponsePending diatur atau tidak. |
| [setResume(Date value)](#setResume-java.util.Date-) | Mengatur nilai Resume. |
| [setSV(double value)](#setSV-double-) | Mengatur nilai SV. |
| [setStart(Date value)](#setStart-java.util.Date-) | Mengatur nilai Start. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | Mengatur nilai StartVariance. |
| [setStop(Date value)](#setStop-java.util.Date-) | Mengatur nilai Stop. |
| [setSummary(boolean value)](#setSummary-boolean-) | Mengatur nilai yang menunjukkan apakah Summary diatur atau tidak. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | Tugas yang diberikan kepada sumber daya. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Mengatur instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi elemen `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) kelas. |
| [setUid(int value)](#setUid-int-) | Mengatur nilai dari Uid. |
| [setUnits(double value)](#setUnits-double-) | Mengatur nilai Units. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | Mengatur nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak. |
| [setVAC(double value)](#setVAC-double-) | Mengatur nilai VAC. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Mengatur nilai dari Work. |
| [setWorkContour(int value)](#setWorkContour-int-) | Mengatur nilai WorkContour. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | Mengatur nilai dari WorkVariance. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Membagi tugas menjadi dua bagian. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Menghasilkan daftar data berfase waktu berdasarkan durasi tugas dan tanggal mulai yang dijadwalkan. |
| [toString()](#toString--) | Mengembalikan representasi string singkat dari instance kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Mengembalikan nilai yang dipetakan ke properti dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Asn](../../com.aspose.tasks/asn) untuk mendapatkan kunci properti. |

**Returns:**
T - nilai yang dipetakan ke properti ini dalam kontainer ini.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Memetakan properti yang ditentukan ke nilai yang ditentukan dalam kontainer ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | kunci properti yang ditentukan. [Asn](../../com.aspose.tasks/asn) untuk mendapatkan kunci properti. |
| val | T | nilai. |

### delete() {#delete--}
```
public final void delete()
```


Menghapus penugasan sumber daya dari koleksi penugasan proyek.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan instance tertentu dari kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Instance [ResourceAssignment](../../com.aspose.tasks/resourceassignment) yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika instance [ResourceAssignment](../../com.aspose.tasks/resourceassignment) yang ditentukan memiliki nilai UID yang sama dengan instance ini; jika tidak, **false**.
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
boolean - **True** jika o adalah ResourceAssignment yang menugaskan sumber daya dan tugas yang sama dengan instance ini; jika tidak, **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


Memperoleh nilai ACWP.

**Returns:**
double - nilai ACWP.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


Memperoleh nilai ActualCost.

**Returns:**
java.math.BigDecimal - nilai ActualCost.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


Mendapatkan nilai ActualFinish.

**Returns:**
java.util.Date - nilai ActualFinish.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


Mendapatkan nilai ActualStart.

**Returns:**
java.util.Date - nilai ActualStart.
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
public final AssignmentBaselineCollection getBaselines()
```


Mendapatkan objek AssignmentBaselineCollection. Kumpulan nilai baseline yang terkait dengan penugasan.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Mendapatkan nilai yang menunjukkan apakah Confirmed diatur atau tidak.

**Returns:**
boolean - nilai yang menunjukkan apakah Confirmed diatur atau tidak.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Mendapatkan nilai Cost.

**Returns:**
java.math.BigDecimal - sebuah nilai dari Cost.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


Mendapatkan nilai CostRateTableType.

**Returns:**
int - nilai CostRateTableType.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Mendapatkan nilai Delay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Mendapatkan instance dari kelas ExtendedAttributeCollection untuk objek ini.

--------------------

Membaca didukung hanya untuk format XML.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Mendapatkan nilai Finish.

**Returns:**
java.util.Date - sebuah nilai dari Finish.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


Mendapatkan nilai FinishVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


Mendapatkan nilai yang menunjukkan apakah FixedMaterial diatur atau tidak.

**Returns:**
boolean - nilai yang menunjukkan apakah FixedMaterial diatur atau tidak.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Mendapatkan pengidentifikasi unik untuk penugasan ini.

**Returns:**
java.util.UUID - pengidentifikasi unik untuk penugasan ini.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Mendapatkan nilai Hyperlink.

**Returns:**
java.lang.String - nilai Hyperlink.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


Mendapatkan nilai HyperlinkAddress.

**Returns:**
java.lang.String - nilai HyperlinkAddress.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


Mendapatkan nilai HyperlinkSubAddress.

**Returns:**
java.lang.String - sebuah nilai dari HyperlinkSubAddress.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Dicadangkan untuk penggunaan internal.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \\{@inheritDoc\\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


Mendapatkan nilai LevelingDelay.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


Mendapatkan nilai yang menunjukkan apakah LinkedFields diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah LinkedFields diatur atau tidak.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Mendapatkan nilai yang menunjukkan apakah Milestone diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah Milestone diatur atau tidak.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


Mendapatkan catatan teks dalam format RTF.

--------------------

Hanya didukung untuk format MPP.

**Returns:**
java.lang.String - catatan teks dalam format RTF.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


Mendapatkan teks polos catatan yang diekstrak dari data RTF.

**Returns:**
java.lang.String - teks polos catatan yang diekstrak dari data RTF.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Mendapatkan nilai yang menunjukkan apakah Overallocated diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah Overallocated diatur atau tidak.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


Mendapatkan nilai OvertimeCost.

**Returns:**
java.math.BigDecimal - sebuah nilai OvertimeCost.
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


Mendapatkan proyek induk untuk penugasan ini.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


Mendapatkan nilai RateScale.

**Returns:**
int - sebuah nilai dari RateScale.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


Sumber daya yang ditugaskan ke tugas.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


Mendapatkan nilai yang menunjukkan apakah ResponsePending diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah ResponsePending diatur atau tidak.
### getResume() {#getResume--}
```
public final Date getResume()
```


Mendapatkan nilai Resume.

**Returns:**
java.util.Date - sebuah nilai dari Resume.
### getSV() {#getSV--}
```
public final double getSV()
```


Mendapatkan nilai SV.

**Returns:**
double - sebuah nilai SV.
### getStart() {#getStart--}
```
public final Date getStart()
```


Mendapatkan nilai Start.

**Returns:**
java.util.Date - sebuah nilai Start.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


Mendapatkan nilai StartVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Mendapatkan nilai Stop.

**Returns:**
java.util.Date - sebuah nilai dari Stop.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Mendapatkan nilai yang menunjukkan apakah Summary diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah Summary diatur atau tidak.
### getTask() {#getTask--}
```
public final Task getTask()
```


Tugas yang diberikan kepada sumber daya.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Mendapatkan instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi elemen `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) kelas.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Mengembalikan objek [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) dengan instance `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) kelas dalam tanggal mulai dan akhir yang diberikan dari [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai untuk data berwaktu. |
| akhir | java.util.Date | Tanggal akhir untuk data berwaktu. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Mengembalikan instance kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi instance `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) kelas dalam tanggal mulai dan akhir yang diberikan dari [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai untuk data berwaktu. |
| akhir | java.util.Date | Tanggal akhir untuk data berwaktu. |
| timephasedType | byte | Tipe data berwaktu ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Mendapatkan jumlah kerja timephased untuk interval tanggal waktu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Awal interval tanggal dan waktu. |
| akhir | java.util.Date | Akhir interval tanggal dan waktu. |

**Returns:**
double - jumlah pekerjaan berwaktu fase untuk interval tanggal dan waktu yang ditentukan.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Mendapatkan jumlah kerja timephased untuk interval tanggal waktu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Awal interval tanggal dan waktu. |
| akhir | java.util.Date | Akhir interval tanggal dan waktu. |
| timephasedDataType | byte | Jenis data berwaktu fase yang akan digunakan. |

**Returns:**
double - jumlah pekerjaan berwaktu fase untuk interval tanggal dan waktu yang ditentukan.
### getUid() {#getUid--}
```
public final int getUid()
```


Mendapatkan nilai Uid.

**Returns:**
int - nilai dari Uid.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Mendapatkan nilai Units.

**Returns:**
double - sebuah nilai dari Units.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


Mendapatkan nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


Mendapatkan nilai VAC.

**Returns:**
double - sebuah nilai dari VAC.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Mendapatkan nilai Work.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


Mendapatkan nilai WorkContour.

**Returns:**
int - sebuah nilai dari WorkContour.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


Mendapatkan nilai WorkVariance.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Mendapatkan nilai yang menunjukkan bahwa penugasan sumber daya ini memiliki anak.

**Returns:**
boolean - Selalu false.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


Mendapatkan nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak.

**Returns:**
boolean - sebuah nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Menghasilkan daftar data berfase waktu.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai yang ditentukan. |
| time | double | Waktu kerja yang ditentukan. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Kalender kerja yang ditentukan. |
| daftar | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | Daftar data berfase waktu. |
| isWorking | boolean | Bendera yang ditentukan yang menunjukkan apakah data berfase waktu berfungsi atau tidak. |
| type | int | Tipe data berfase waktu yang ditentukan. |

**Returns:**
java.util.Date - Tanggal maksimum dari daftar atau tanggal mulai jika daftar kosong.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


Mengatur nilai ACWP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari ACWP. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


Mengatur nilai ActualCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari ActualCost. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


Mengatur nilai ActualFinish.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai ActualFinish. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


Mengatur nilai ActualStart.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai ActualStart. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Mengatur nilai yang menunjukkan apakah Confirmed diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Confirmed diatur atau tidak. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Mengatur nilai Cost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai dari Cost. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


Mengatur nilai CostRateTableType.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai CostRateTableType. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Mengatur nilai Delay.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai Delay. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Mengatur sebuah instance kelas ExtendedAttributeCollection untuk objek ini.

--------------------

Membaca didukung hanya untuk format XML.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | sebuah instance dari kelas ExtendedAttributeCollection untuk objek ini. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Mengatur nilai Finish.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Finish. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


Mengatur nilai FinishVariance.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai FinishVariance. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


Mengatur nilai yang menunjukkan apakah FixedMaterial diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah FixedMaterial diatur atau tidak. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


Mengatur nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah HasFixedRateUnits diatur atau tidak. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Mengatur pengidentifikasi unik untuk penugasan ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.UUID | pengidentifikasi unik untuk penugasan ini. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Mengatur nilai Hyperlink.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai Hyperlink. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


Mengatur nilai HyperlinkAddress.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai HyperlinkAddress. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


Mengatur nilai HyperlinkSubAddress.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nilai HyperlinkSubAddress. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


Mengatur nilai LevelingDelay.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai LevelingDelay. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


Mengatur nilai yang menunjukkan apakah LinkedFields diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah LinkedFields diatur atau tidak. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Menetapkan satuan untuk penugasan sumber daya material dengan konsumsi material variabel. Konsumsi material variabel berarti bahwa seiring perubahan durasi penugasan, jumlah material yang digunakan berubah secara proporsional.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| unit | double | Jumlah unit yang diakumulasi pada periode waktu. |
|  | rateScaleType | int | Periode waktu di mana nilai unit diakumulasi. |

--------------------

Sebagai contoh, untuk mengatur '123/bulan', SetUnitsScaled(123D, RateScaleType.Month) harus dipanggil. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Mengatur nilai yang menunjukkan apakah Milestone diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Milestone diatur atau tidak. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Mengatur catatan teks dalam format RTF.

--------------------

Hanya didukung untuk format MPP.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | catatan teks dalam format RTF. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


Mengatur teks polos catatan yang diekstrak dari data RTF.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | teks polos catatan yang diekstrak dari data RTF. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Mengatur nilai yang menunjukkan apakah Overallocated diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Overallocated diatur atau tidak. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


Mengatur nilai OvertimeCost.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.math.BigDecimal | nilai OvertimeCost. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


Mengatur nilai RateScale.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari RateScale. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


Sumber daya yang ditugaskan ke tugas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | sumber daya yang ditugaskan ke sebuah tugas. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


Mengatur nilai yang menunjukkan apakah ResponsePending diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah ResponsePending diatur atau tidak. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Mengatur nilai Resume.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Resume. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


Mengatur nilai SV.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai SV. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Mengatur nilai Start.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Start. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


Mengatur nilai StartVariance.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari StartVariance. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Mengatur nilai Stop.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | nilai dari Stop. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Mengatur nilai yang menunjukkan apakah Summary diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah Summary diatur atau tidak. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


Tugas yang diberikan kepada sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | tugas yang mana sumber daya ditugaskan. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Mengatur instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi elemen `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) kelas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | instance dari kelas [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) yang berisi elemen `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)). |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Mengatur nilai dari Uid.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari Uid. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Mengatur nilai Units.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari Units. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


Mengatur nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah UpdateNeeded diatur atau tidak. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


Mengatur nilai VAC.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | nilai dari VAC. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Mengatur nilai dari Work.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari Work. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


Mengatur nilai WorkContour.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | nilai dari WorkContour. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


Mengatur nilai dari WorkVariance.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | nilai dari WorkVariance. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Membagi tugas menjadi dua bagian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Awal gangguan kerja untuk dibagi berdasarkan. |
| selesai | java.util.Date | Akhir gangguan kerja untuk dibagi berdasarkan. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Kalender untuk dibagi berdasarkan. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Menghasilkan daftar data berfase waktu berdasarkan durasi tugas dan tanggal mulai yang dijadwalkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Kalender untuk menghasilkan data berfase waktu. |

### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string pendek dari instance kelas [ResourceAssignment](../../com.aspose.tasks/resourceassignment). Detail tepat dari representasi tidak ditentukan dan dapat berubah.

**Returns:**
java.lang.String - string pendek yang mewakili objek penugasan.

---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projede bir kaynak atamasını temsil eder."
type: docs
weight: 249
url: /tr/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

Projede bir kaynak atamasını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | Bu konteynerde özelliğin eşlendiği değeri döndürür. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | Belirtilen özelliği bu konteynerde belirtilen değere eşler. |
| [delete()](#delete--) | Kaynak atamasını proje atamaları koleksiyonundan siler. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | Bu örneğin, [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [getACWP()](#getACWP--) | ACWP değerini alır. |
| [getActualCost()](#getActualCost--) | ActualCost değerini alır. |
| [getActualFinish()](#getActualFinish--) | ActualFinish değerini alır. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost değerini alır. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork değerini alır. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected değerini alır. |
| [getActualStart()](#getActualStart--) | ActualStart değerini alır. |
| [getActualWork()](#getActualWork--) | ActualWork değerini alır. |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected değerini alır. |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner değerini alır. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid değerini alır. |
| [getBCWP()](#getBCWP--) | BCWP değerini alır. |
| [getBCWS()](#getBCWS--) | BCWS değerini alır. |
| [getBaselines()](#getBaselines--) | AssignmentBaselineCollection nesnesini alır. |
| [getBookingType()](#getBookingType--) | BookingType değerini alır. |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost değerini alır. |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork değerini alır. |
| [getCV()](#getCV--) | CV değerini alır. |
| [getConfirmed()](#getConfirmed--) | Confirmed'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getCost()](#getCost--) | Cost değerini alır. |
| [getCostRateTableType()](#getCostRateTableType--) | CostRateTableType değerini alır. |
| [getCostVariance()](#getCostVariance--) | CostVariance değerini alır. |
| [getCreated()](#getCreated--) | Created değerini alır. |
| [getDelay()](#getDelay--) | Delay değerini alır. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini alır. |
| [getFinish()](#getFinish--) | Finish değerini alır. |
| [getFinishVariance()](#getFinishVariance--) | FinishVariance değerini alır. |
| [getFixedMaterial()](#getFixedMaterial--) | FixedMaterial'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getGuid()](#getGuid--) | Bu atama için benzersiz tanımlayıcı alır. |
| [getHyperlink()](#getHyperlink--) | Hyperlink'in değerini alır. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | HyperlinkAddress'in değerini alır. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | HyperlinkSubAddress'in değerini alır. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | LevelingDelay'in değerini alır. |
| [getLinkedFields()](#getLinkedFields--) | LinkedFields'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getMilestone()](#getMilestone--) | Milestone'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getNotesRTF()](#getNotesRTF--) | RTF biçimindeki metin notlarını alır. |
| [getNotesText()](#getNotesText--) | RTF verilerinden çıkarılan notların düz metnini alır. |
| [getOverallocated()](#getOverallocated--) | Overallocated'in ayarlanıp ayarlanmadığını gösteren değeri alır. |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost değerini alır. |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork değerini alır. |
| [getParentProject()](#getParentProject--) | Bu atama için üst proje alır. |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits değerini alır. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete değerini alır. |
| [getRateScale()](#getRateScale--) | RateScale'in değerini alır. |
| [getRegularWork()](#getRegularWork--) | RegularWork değerini alır. |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost değerini alır. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost değerini alır. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork değerini alır. |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork değerini alır. |
| [getResource()](#getResource--) | Bir göreve atanan kaynak. |
| [getResponsePending()](#getResponsePending--) | ResponsePending'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getResume()](#getResume--) | Resume'un değerini alır. |
| [getSV()](#getSV--) | SV değerini alır. |
| [getStart()](#getStart--) | Start değerini alır. |
| [getStartVariance()](#getStartVariance--) | StartVariance'in değerini alır. |
| [getStop()](#getStop--) | Stop'un değerini alır. |
| [getSummary()](#getSummary--) | Summary'nin ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getTask()](#getTask--) | Bir kaynağın atandığı görev. |
| [getTimephasedData()](#getTimephasedData--) | Elemanları `TimephasedData` içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının örneğini alır. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | Verilen başlangıç ve bitiş tarihleri içinde [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) için `TimephasedData` örneklerini içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) nesnesini döndürür. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | Belirtilen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) için verilen başlangıç ve bitiş tarihleri içinde `TimephasedData` örneklerini içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının örneğini döndürür. |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır. |
| [getUid()](#getUid--) | Uid değerini alır. |
| [getUnits()](#getUnits--) | Units'in değerini alır. |
| [getUpdateNeeded()](#getUpdateNeeded--) | UpdateNeeded'ın ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [getVAC()](#getVAC--) | VAC'in değerini alır. |
| [getWork()](#getWork--) | Work değerini alır. |
| [getWorkContour()](#getWorkContour--) | WorkContour'in değerini alır. |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance değerini alır. |
| [hasChildren()](#hasChildren--) | Bu kaynak atamasının alt öğeleri olduğunu gösteren bir değer alır. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | HasFixedRateUnits'in ayarlanıp ayarlanmadığını gösteren bir değer alır. |
| [hashCode()](#hashCode--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının örneği için bir karma kod değeri döndürür. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | Zaman aşamalı verilerin bir listesini oluşturur. |
| [setACWP(double value)](#setACWP-double-) | ACWP değerini ayarlar. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost değerini ayarlar. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | ActualFinish değerini ayarlar. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost değerini ayarlar. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork değerini ayarlar. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected değerini ayarlar. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | ActualStart değerini ayarlar. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork değerini ayarlar. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected değerini ayarlar. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner değerini ayarlar. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid değerini ayarlar. |
| [setBCWP(double value)](#setBCWP-double-) | BCWP değerini ayarlar. |
| [setBCWS(double value)](#setBCWS-double-) | BCWS değerini ayarlar. |
| [setBookingType(int value)](#setBookingType-int-) | BookingType'in değerini ayarlar. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost'in değerini ayarlar. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork'in değerini ayarlar. |
| [setCV(double value)](#setCV-double-) | CV'in değerini ayarlar. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Confirmed'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost'un değerini ayarlar. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | CostRateTableType değerini ayarlar. |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance'ın değerini ayarlar. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created'ın değerini ayarlar. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Delay değerini ayarlar. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini ayarlar. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish'in değerini ayarlar. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | FinishVariance değerini ayarlar. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | FixedMaterial'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | HasFixedRateUnits'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | Bu atama için benzersiz tanımlayıcıyı ayarlar. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Hyperlink değerini ayarlar. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | HyperlinkAddress değerini ayarlar. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | HyperlinkSubAddress değerini ayarlar. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | LevelingDelay değerini ayarlar. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | LinkedFields'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | Değişken malzeme tüketimine sahip bir malzeme kaynağının ataması için birimleri ayarlar. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Milestone'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | Metin notlarını RTF formatında ayarlar. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | RTF verilerinden çıkarılan notların düz metnini ayarlar. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Overallocated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost'in değerini ayarlar. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork'in değerini ayarlar. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits'in değerini ayarlar. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete'in değerini ayarlar. |
| [setRateScale(int value)](#setRateScale-int-) | RateScale değerini ayarlar. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork'in değerini ayarlar. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost'in değerini ayarlar. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost'in değerini ayarlar. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork'in değerini ayarlar. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork'in değerini ayarlar. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | Bir göreve atanan kaynak. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | ResponsePending'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar. |
| [setResume(Date value)](#setResume-java.util.Date-) | Resume değerini ayarlar. |
| [setSV(double value)](#setSV-double-) | SV'in değerini ayarlar. |
| [setStart(Date value)](#setStart-java.util.Date-) | Start'in değerini ayarlar. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | StartVariance değerini ayarlar. |
| [setStop(Date value)](#setStop-java.util.Date-) | Stop değerini ayarlar. |
| [setSummary(boolean value)](#setSummary-boolean-) | Summary'nin ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | Bir kaynağın atandığı görev. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının öğeleri `TimephasedData` içeren örneğini ayarlar ([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) sınıfı. |
| [setUid(int value)](#setUid-int-) | Uid değerini ayarlar. |
| [setUnits(double value)](#setUnits-double-) | Units değerini ayarlar. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | UpdateNeeded'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar. |
| [setVAC(double value)](#setVAC-double-) | VAC değerini ayarlar. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work değerini ayarlar. |
| [setWorkContour(int value)](#setWorkContour-int-) | WorkContour değerini ayarlar. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | WorkVariance değerini ayarlar. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | Görevi iki parçaya böler. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | Görev süresi ve planlanan başlangıç tarihine göre zaman aşamalı veri listesini oluşturur. |
| [toString()](#toString--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının örneğinin kısa dize temsilini döndürür. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


Bu konteynerde özelliğin eşlendiği değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | belirtilen özellik anahtarı. Özellik anahtarını almak için [Asn](../../com.aspose.tasks/asn). |

**Returns:**
T - bu kapsayıcıda özelliğin eşlendiği değer.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


Belirtilen özelliği bu konteynerde belirtilen değere eşler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | belirtilen özellik anahtarı. Özellik anahtarını almak için [Asn](../../com.aspose.tasks/asn). |
| değer. | T | değer. |

### delete() {#delete--}
```
public final void delete()
```


Kaynak atamasını proje atamaları koleksiyonundan siler.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


Bu örneğin, [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının belirtilen bir örneğiyle eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Bu örnek ile karşılaştırmak için belirtilen [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfı örneği. |

**Returns:**
boolean - **True** eğer belirtilen [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının örneği bu örnekle aynı UID değerine sahipse; aksi takdirde **false**.
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
boolean - **True** eğer o, bu örnekle aynı kaynağı ve görevi atayan bir ResourceAssignment ise; aksi takdirde **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP değerini alır.

**Returns:**
double - ACWP değerini.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost değerini alır.

**Returns:**
java.math.BigDecimal - ActualCost değerini.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


ActualFinish değerini alır.

**Returns:**
java.util.Date - ActualFinish değerinin bir değeri.
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
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


ActualStart değerini alır.

**Returns:**
java.util.Date - ActualStart değerinin bir değeri.
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
public final AssignmentBaselineCollection getBaselines()
```


AssignmentBaselineCollection nesnesini alır. Bir atamayla ilişkili temel değerlerin koleksiyonu.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
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
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Confirmed'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - Confirmed'in ayarlanıp ayarlanmadığını belirten bir değer.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost değerini alır.

**Returns:**
java.math.BigDecimal - Cost değerinin bir değeri.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


CostRateTableType değerini alır.

**Returns:**
int - CostRateTableType değerinin bir değeri.
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
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Delay değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini alır.

--------------------

Okuma yalnızca XML formatı için desteklenir.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish değerini alır.

**Returns:**
java.util.Date - Finish değerinin bir değeri.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


FinishVariance değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


FixedMaterial'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - FixedMaterial'in ayarlanıp ayarlanmadığını belirten bir değer.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Bu atama için benzersiz tanımlayıcı alır.

**Returns:**
java.util.UUID - bu atama için benzersiz tanımlayıcı.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hyperlink'in değerini alır.

**Returns:**
java.lang.String - Hyperlink değerinin bir değeri.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


HyperlinkAddress'in değerini alır.

**Returns:**
java.lang.String - HyperlinkAddress değerinin bir değeri.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


HyperlinkSubAddress'in değerini alır.

**Returns:**
java.lang.String - HyperlinkSubAddress değeri.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


Dahili kullanım için ayrılmıştır.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \{@inheritDoc\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


LevelingDelay'in değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


LinkedFields'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - LinkedFields ayarlı olup olmadığını gösteren bir değer.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Milestone'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - Milestone ayarlı olup olmadığını gösteren bir değer.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


RTF biçimindeki metin notlarını alır.

--------------------

Yalnızca MPP formatları için desteklenir.

**Returns:**
java.lang.String - RTF formatındaki metin notları.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


RTF verilerinden çıkarılan notların düz metnini alır.

**Returns:**
java.lang.String - RTF verilerinden çıkarılan notların düz metni.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Overallocated'in ayarlanıp ayarlanmadığını gösteren değeri alır.

**Returns:**
boolean - Overallocated ayarlı olup olmadığını gösteren bir değer.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost değerini alır.

**Returns:**
java.math.BigDecimal - OvertimeCost'in bir değeri.
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


Bu atama için üst proje alır.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
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
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


RateScale'in değerini alır.

**Returns:**
int - RateScale değeri.
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
### getResource() {#getResource--}
```
public final Resource getResource()
```


Bir göreve atanan kaynak.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


ResponsePending'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - ResponsePending ayarlı olup olmadığını gösteren bir değer.
### getResume() {#getResume--}
```
public final Date getResume()
```


Resume'un değerini alır.

**Returns:**
java.util.Date - Resume değeri.
### getSV() {#getSV--}
```
public final double getSV()
```


SV değerini alır.

**Returns:**
double - SV'nin bir değeri.
### getStart() {#getStart--}
```
public final Date getStart()
```


Start değerini alır.

**Returns:**
java.util.Date - Start'ın bir değeri.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


StartVariance'in değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Stop'un değerini alır.

**Returns:**
java.util.Date - Stop değeri.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Summary'nin ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - Summary ayarlı olup olmadığını gösteren bir değer.
### getTask() {#getTask--}
```
public final Task getTask()
```


Bir kaynağın atandığı görev.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Elemanları `TimephasedData` içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının örneğini alır.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


Verilen başlangıç ve bitiş tarihleri içinde [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork) için `TimephasedData` örneklerini içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) nesnesini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Zaman aşamalı veriler için başlangıç tarihi. |
| bitiş | java.util.Date | Zaman aşamalı veriler için bitiş tarihi. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


Belirtilen [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype) için verilen başlangıç ve bitiş tarihleri içinde `TimephasedData` örneklerini içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının örneğini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Zaman aşamalı veriler için başlangıç tarihi. |
| bitiş | java.util.Date | Zaman aşamalı veriler için bitiş tarihi. |
| timephasedType | byte | Zaman aşamalı verilerin türü ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Tarih saat aralığının başlangıcı. |
| bitiş | java.util.Date | Tarih saat aralığının sonu. |

**Returns:**
double - belirtilen tarih saat aralığı için zaman aşamalı iş miktarı.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


Belirtilen tarih zaman aralığı için zaman aşamalı iş miktarını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Tarih saat aralığının başlangıcı. |
| bitiş | java.util.Date | Tarih saat aralığının sonu. |
| timephasedDataType | byte | Kullanılacak zaman aşamalı verinin türü. |

**Returns:**
double - belirtilen tarih saat aralığı için zaman aşamalı iş miktarı.
### getUid() {#getUid--}
```
public final int getUid()
```


Uid değerini alır.

**Returns:**
int - Uid değerinin bir değeri.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Units'in değerini alır.

**Returns:**
double - Units değeri.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


UpdateNeeded'ın ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - UpdateNeeded ayarlı olup olmadığını gösteren bir değer.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


VAC'in değerini alır.

**Returns:**
double - VAC değeri.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


WorkContour'in değerini alır.

**Returns:**
int - WorkContour değeri.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


WorkVariance değerini alır.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


Bu kaynak atamasının alt öğeleri olduğunu gösteren bir değer alır.

**Returns:**
boolean - Her zaman false.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


HasFixedRateUnits'in ayarlanıp ayarlanmadığını gösteren bir değer alır.

**Returns:**
boolean - HasFixedRateUnits ayarlı olup olmadığını gösteren bir değer.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfının örneği için bir karma kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


Zaman aşamalı verilerin bir listesini oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Belirtilen başlangıç tarihi. |
| time | double | Belirtilen çalışma süresi. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Belirtilen çalışma takvimi. |
| liste | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | Zaman aşamalı verilerin listesi. |
| isWorking | boolean | Zaman aşamalı verilerin çalışıp çalışmadığını belirten belirtilen bayrak. |
| tür | int | Belirtilen zaman aşamalı veri türü. |

**Returns:**
java.util.Date - Listeden maksimum tarih veya liste boşsa başlangıç tarihi.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | ACWP değerinin bir değeri. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | ActualCost değerinin bir değeri. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


ActualFinish değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | ActualFinish değeri. |

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

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


ActualStart değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | ActualStart değeri. |

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

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Confirmed'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Confirmed ayarlanıp ayarlanmadığını gösteren değer. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost'un değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | Cost'un bir değeri. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


CostRateTableType değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | CostRateTableType değeri. |

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

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Delay değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Delay değeri. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


Bu nesne için ExtendedAttributeCollection sınıfının bir örneğini ayarlar.

--------------------

Okuma yalnızca XML formatı için desteklenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | Bu nesne için ExtendedAttributeCollection sınıfının bir örneği. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Finish'ın bir değeri. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


FinishVariance değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | FinishVariance değeri. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


FixedMaterial'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | FixedMaterial ayarlanıp ayarlanmadığını gösteren değer. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


HasFixedRateUnits'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | HasFixedRateUnits ayarlanıp ayarlanmadığını gösteren değer. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Bu atama için benzersiz tanımlayıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.UUID | Bu atama için benzersiz tanımlayıcı. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Hyperlink değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Hyperlink değeri. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


HyperlinkAddress değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | HyperlinkAddress değeri. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


HyperlinkSubAddress değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | HyperlinkSubAddress değeri. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


LevelingDelay değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | LevelingDelay değeri. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


LinkedFields'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | LinkedFields ayarlanıp ayarlanmadığını gösteren değer. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


Değişken malzeme tüketimine sahip bir malzeme kaynağının ataması için birimleri ayarlar. Değişken malzeme tüketimi, atama süresi değiştikçe kullanılan malzeme miktarının orantılı olarak değişmesi anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| birimler | double | Zaman diliminde biriken birim sayısı. |
|  | rateScaleType | int | Birim değerinin biriktiği zaman dilimi. |

--------------------

Örneğin, '123/ay' ayarlamak için, SetUnitsScaled(123D, RateScaleType.Month) çağrılmalıdır. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Milestone'ın ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Milestone'un ayarlanıp ayarlanmadığını gösteren bir değer. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


Metin notlarını RTF formatında ayarlar.

--------------------

Yalnızca MPP formatları için desteklenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | RTF formatındaki metin notları. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


RTF verilerinden çıkarılan notların düz metnini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | RTF verilerinden çıkarılan notların düz metni. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Overallocated'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Overallocated'in ayarlanıp ayarlanmadığını gösteren değer. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.math.BigDecimal | OvertimeCost değeri. |

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

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


RateScale değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | RateScale'in bir değeri. |

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

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


Bir göreve atanan kaynak.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | Bir göreve atanan kaynak. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


ResponsePending'in ayarlanıp ayarlanmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | ResponsePending'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Resume değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Resume'un bir değeri. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | SV değeri. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start'in değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Start'ın bir değeri. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


StartVariance değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | StartVariance'in bir değeri. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Stop değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | Stop'un bir değeri. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Summary'nin ayarlanıp ayarlanmadığını belirten bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Summary'nin ayarlanıp ayarlanmadığını gösteren bir değer. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


Bir kaynağın atandığı görev.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | Kaynağın atandığı görev. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının öğeleri `TimephasedData` içeren örneğini ayarlar ([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) sınıfı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | Öğeleri `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) içeren [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) sınıfının bir örneği. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Uid'nin bir değeri. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Units değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | Units'ın bir değeri. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


UpdateNeeded'in ayarlanıp ayarlanmadığını belirten bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | UpdateNeeded'in ayarlanıp ayarlanmadığını gösteren bir değer. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


VAC değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double | VAC'ın bir değeri. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work'in bir değeri. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


WorkContour değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | WorkContour'ın bir değeri. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


WorkVariance değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | WorkVariance'ın bir değeri. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


Görevi iki parçaya böler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlat | java.util.Date | Bölünecek çalışma kesintisinin başlangıcı. |
| bitiş | java.util.Date | Bölünecek çalışma kesintisinin sonu. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Bölünme için kullanılan takvim. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


Görev süresi ve planlanan başlangıç tarihine göre zaman aşamalı veri listesini oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | Zaman aşamalı verileri oluşturmak için kullanılan takvim. |

### toString() {#toString--}
```
public String toString()
```


Bir [ResourceAssignment](../../com.aspose.tasks/resourceassignment) sınıfı örneğinin kısa dize temsilini döndürür. Temsilin kesin ayrıntıları belirtilmemiştir ve değişikliğe açıktır.

**Returns:**
java.lang.String - atama nesnesini temsil eden kısa dize.

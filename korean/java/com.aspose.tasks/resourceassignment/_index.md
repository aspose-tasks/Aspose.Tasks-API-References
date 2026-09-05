---
title: "ResourceAssignment"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트의 리소스 할당을 나타냅니다."
type: docs
weight: 249
url: /ko/java/com.aspose.tasks/resourceassignment/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable, com.aspose.tasks.IExtendedAttributeParent, com.aspose.tasks.IEntityWithNotes, com.aspose.tasks.IEntityWithHyperlink
```
public class ResourceAssignment extends IContainer<Byte> implements System.IEquatable<ResourceAssignment>, IExtendedAttributeParent, IEntityWithNotes, IEntityWithHyperlink
```

프로젝트의 리소스 할당을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 이 컨테이너에서 속성이 매핑된 값을 반환합니다. |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다. |
| [delete()](#delete--) | 프로젝트 할당 컬렉션에서 리소스 할당을 삭제합니다. |
| [equals(ResourceAssignment other)](#equals-com.aspose.tasks.ResourceAssignment-) | 이 인스턴스가 지정된 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스 인스턴스와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getACWP()](#getACWP--) | ACWP 값을 가져옵니다. |
| [getActualCost()](#getActualCost--) | ActualCost 값을 가져옵니다. |
| [getActualFinish()](#getActualFinish--) | ActualFinish 값을 가져옵니다. |
| [getActualOvertimeCost()](#getActualOvertimeCost--) | ActualOvertimeCost 값을 가져옵니다. |
| [getActualOvertimeWork()](#getActualOvertimeWork--) | ActualOvertimeWork 값을 가져옵니다. |
| [getActualOvertimeWorkProtected()](#getActualOvertimeWorkProtected--) | ActualOvertimeWorkProtected 값을 가져옵니다. |
| [getActualStart()](#getActualStart--) | ActualStart 값을 가져옵니다. |
| [getActualWork()](#getActualWork--) | ActualWork 값을 가져옵니다. |
| [getActualWorkProtected()](#getActualWorkProtected--) | ActualWorkProtected 값을 가져옵니다. |
| [getAssignmentOwner()](#getAssignmentOwner--) | AssignmentOwner 값을 가져옵니다. |
| [getAssignmentOwnerGuid()](#getAssignmentOwnerGuid--) | AssignmentOwnerGuid 값을 가져옵니다. |
| [getBCWP()](#getBCWP--) | BCWP 값을 가져옵니다. |
| [getBCWS()](#getBCWS--) | BCWS 값을 가져옵니다. |
| [getBaselines()](#getBaselines--) | AssignmentBaselineCollection 객체를 가져옵니다. |
| [getBookingType()](#getBookingType--) | BookingType 값을 가져옵니다. |
| [getBudgetCost()](#getBudgetCost--) | BudgetCost 값을 가져옵니다. |
| [getBudgetWork()](#getBudgetWork--) | BudgetWork 값을 가져옵니다. |
| [getCV()](#getCV--) | CV 값을 가져옵니다. |
| [getConfirmed()](#getConfirmed--) | Confirmed가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getCost()](#getCost--) | Cost의 값을 가져옵니다. |
| [getCostRateTableType()](#getCostRateTableType--) | CostRateTableType 값을 가져옵니다. |
| [getCostVariance()](#getCostVariance--) | CostVariance의 값을 가져옵니다. |
| [getCreated()](#getCreated--) | Created의 값을 가져옵니다. |
| [getDelay()](#getDelay--) | Delay 값을 가져옵니다. |
| [getExtendedAttributes()](#getExtendedAttributes--) | 이 객체에 대한 ExtendedAttributeCollection 클래스의 인스턴스를 가져옵니다. |
| [getFinish()](#getFinish--) | Finish의 값을 가져옵니다. |
| [getFinishVariance()](#getFinishVariance--) | FinishVariance 값을 가져옵니다. |
| [getFixedMaterial()](#getFixedMaterial--) | FixedMaterial이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getGuid()](#getGuid--) | 이 할당에 대한 고유 식별자를 가져옵니다. |
| [getHyperlink()](#getHyperlink--) | Hyperlink 값을 가져옵니다. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | HyperlinkAddress 값을 가져옵니다. |
| [getHyperlinkSubAddress()](#getHyperlinkSubAddress--) | HyperlinkSubAddress 값을 가져옵니다. |
| [getItems()](#getItems--) | \{@inheritDoc\} |
| [getLevelingDelay()](#getLevelingDelay--) | LevelingDelay 값을 가져옵니다. |
| [getLinkedFields()](#getLinkedFields--) | LinkedFields가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getMilestone()](#getMilestone--) | Milestone이 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getNotesRTF()](#getNotesRTF--) | RTF 형식의 텍스트 메모를 가져옵니다. |
| [getNotesText()](#getNotesText--) | RTF 데이터에서 추출된 메모의 일반 텍스트를 가져옵니다. |
| [getOverallocated()](#getOverallocated--) | Overallocated가 설정되었는지 여부를 나타내는 값을 가져옵니다. |
| [getOvertimeCost()](#getOvertimeCost--) | OvertimeCost의 값을 가져옵니다. |
| [getOvertimeWork()](#getOvertimeWork--) | OvertimeWork의 값을 가져옵니다. |
| [getParentProject()](#getParentProject--) | 이 할당에 대한 상위 프로젝트를 가져옵니다. |
| [getPeakUnits()](#getPeakUnits--) | PeakUnits의 값을 가져옵니다. |
| [getPercentWorkComplete()](#getPercentWorkComplete--) | PercentWorkComplete의 값을 가져옵니다. |
| [getRateScale()](#getRateScale--) | RateScale 값을 가져옵니다. |
| [getRegularWork()](#getRegularWork--) | RegularWork의 값을 가져옵니다. |
| [getRemainingCost()](#getRemainingCost--) | RemainingCost의 값을 가져옵니다. |
| [getRemainingOvertimeCost()](#getRemainingOvertimeCost--) | RemainingOvertimeCost의 값을 가져옵니다. |
| [getRemainingOvertimeWork()](#getRemainingOvertimeWork--) | RemainingOvertimeWork의 값을 가져옵니다. |
| [getRemainingWork()](#getRemainingWork--) | RemainingWork의 값을 가져옵니다. |
| [getResource()](#getResource--) | 작업에 할당된 자원. |
| [getResponsePending()](#getResponsePending--) | ResponsePending가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getResume()](#getResume--) | Resume 값을 가져옵니다. |
| [getSV()](#getSV--) | SV의 값을 가져옵니다. |
| [getStart()](#getStart--) | Start의 값을 가져옵니다. |
| [getStartVariance()](#getStartVariance--) | StartVariance 값을 가져옵니다. |
| [getStop()](#getStop--) | Stop 값을 가져옵니다. |
| [getSummary()](#getSummary--) | Summary가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getTask()](#getTask--) | 리소스가 할당된 작업. |
| [getTimephasedData()](#getTimephasedData--) | TimephasedData 요소(`TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)))를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 가져옵니다. |
| [getTimephasedData(Date start, Date end)](#getTimephasedData-java.util.Date-java.util.Date-) | 주어진 시작 및 종료 날짜의 [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork)에 해당하는 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 인스턴스를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체를 반환합니다. |
| [getTimephasedData(Date start, Date end, byte timephasedType)](#getTimephasedData-java.util.Date-java.util.Date-byte-) | 지정된 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)의 주어진 시작 및 종료 날짜 내에 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 인스턴스를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 반환합니다. |
| [getTimephasedWork(Date start, Date end)](#getTimephasedWork-java.util.Date-java.util.Date-) | 지정된 날짜 및 시간 간격에 대한 시간별 작업량을 가져옵니다. |
| [getTimephasedWork(Date start, Date end, byte timephasedDataType)](#getTimephasedWork-java.util.Date-java.util.Date-byte-) | 지정된 날짜 및 시간 간격에 대한 시간별 작업량을 가져옵니다. |
| [getUid()](#getUid--) | Uid의 값을 가져옵니다. |
| [getUnits()](#getUnits--) | Units 값을 가져옵니다. |
| [getUpdateNeeded()](#getUpdateNeeded--) | UpdateNeeded가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [getVAC()](#getVAC--) | VAC 값을 가져옵니다. |
| [getWork()](#getWork--) | Work의 값을 가져옵니다. |
| [getWorkContour()](#getWorkContour--) | WorkContour 값을 가져옵니다. |
| [getWorkVariance()](#getWorkVariance--) | WorkVariance의 값을 가져옵니다. |
| [hasChildren()](#hasChildren--) | 이 리소스 할당에 하위 항목이 있음을 나타내는 값을 가져옵니다. |
| [hasFixedRateUnits()](#hasFixedRateUnits--) | HasFixedRateUnits가 설정되어 있는지 여부를 나타내는 값을 가져옵니다. |
| [hashCode()](#hashCode--) | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |
| [makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type)](#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-) | 시간별 데이터 목록을 생성합니다. |
| [setACWP(double value)](#setACWP-double-) | ACWP의 값을 설정합니다. |
| [setActualCost(BigDecimal value)](#setActualCost-java.math.BigDecimal-) | ActualCost의 값을 설정합니다. |
| [setActualFinish(Date value)](#setActualFinish-java.util.Date-) | ActualFinish 값을 설정합니다. |
| [setActualOvertimeCost(BigDecimal value)](#setActualOvertimeCost-java.math.BigDecimal-) | ActualOvertimeCost의 값을 설정합니다. |
| [setActualOvertimeWork(Duration value)](#setActualOvertimeWork-com.aspose.tasks.Duration-) | ActualOvertimeWork의 값을 설정합니다. |
| [setActualOvertimeWorkProtected(Duration value)](#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-) | ActualOvertimeWorkProtected의 값을 설정합니다. |
| [setActualStart(Date value)](#setActualStart-java.util.Date-) | ActualStart 값을 설정합니다. |
| [setActualWork(Duration value)](#setActualWork-com.aspose.tasks.Duration-) | ActualWork의 값을 설정합니다. |
| [setActualWorkProtected(Duration value)](#setActualWorkProtected-com.aspose.tasks.Duration-) | ActualWorkProtected의 값을 설정합니다. |
| [setAssignmentOwner(String value)](#setAssignmentOwner-java.lang.String-) | AssignmentOwner의 값을 설정합니다. |
| [setAssignmentOwnerGuid(String value)](#setAssignmentOwnerGuid-java.lang.String-) | AssignmentOwnerGuid의 값을 설정합니다. |
| [setBCWP(double value)](#setBCWP-double-) | BCWP의 값을 설정합니다. |
| [setBCWS(double value)](#setBCWS-double-) | BCWS의 값을 설정합니다. |
| [setBookingType(int value)](#setBookingType-int-) | BookingType의 값을 설정합니다. |
| [setBudgetCost(BigDecimal value)](#setBudgetCost-java.math.BigDecimal-) | BudgetCost의 값을 설정합니다. |
| [setBudgetWork(Duration value)](#setBudgetWork-com.aspose.tasks.Duration-) | BudgetWork의 값을 설정합니다. |
| [setCV(double value)](#setCV-double-) | CV의 값을 설정합니다. |
| [setConfirmed(boolean value)](#setConfirmed-boolean-) | Confirmed가 설정되어 있는지 여부를 나타내는 값을 설정합니다. |
| [setCost(BigDecimal value)](#setCost-java.math.BigDecimal-) | Cost의 값을 설정합니다. |
| [setCostRateTableType(int value)](#setCostRateTableType-int-) | CostRateTableType 값을 설정합니다. |
| [setCostVariance(double value)](#setCostVariance-double-) | CostVariance의 값을 설정합니다. |
| [setCreated(Date value)](#setCreated-java.util.Date-) | Created의 값을 설정합니다. |
| [setDelay(Duration value)](#setDelay-com.aspose.tasks.Duration-) | Delay 값을 설정합니다. |
| [setExtendedAttributes(ExtendedAttributeCollection value)](#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-) | 이 개체에 대해 ExtendedAttributeCollection 클래스의 인스턴스를 설정합니다. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Finish의 값을 설정합니다. |
| [setFinishVariance(Duration value)](#setFinishVariance-com.aspose.tasks.Duration-) | FinishVariance 값을 설정합니다. |
| [setFixedMaterial(boolean value)](#setFixedMaterial-boolean-) | FixedMaterial이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setFixedRateUnits(boolean value)](#setFixedRateUnits-boolean-) | HasFixedRateUnits가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | 이 할당에 대한 고유 식별자를 설정합니다. |
| [setHyperlink(String value)](#setHyperlink-java.lang.String-) | Hyperlink 값을 설정합니다. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | HyperlinkAddress 값을 설정합니다. |
| [setHyperlinkSubAddress(String value)](#setHyperlinkSubAddress-java.lang.String-) | HyperlinkSubAddress 값을 설정합니다. |
| [setLevelingDelay(Duration value)](#setLevelingDelay-com.aspose.tasks.Duration-) | LevelingDelay 값을 설정합니다. |
| [setLinkedFields(boolean value)](#setLinkedFields-boolean-) | LinkedFields가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setMaterialResourceUnits(double units, int rateScaleType)](#setMaterialResourceUnits-double-int-) | 가변 재료 소비가 있는 자재 리소스 할당에 대한 단위를 설정합니다. |
| [setMilestone(boolean value)](#setMilestone-boolean-) | Milestone이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setNotesRTF(String value)](#setNotesRTF-java.lang.String-) | RTF 형식으로 텍스트 메모를 설정합니다. |
| [setNotesText(String value)](#setNotesText-java.lang.String-) | RTF 데이터에서 추출한 메모의 일반 텍스트를 설정합니다. |
| [setOverallocated(boolean value)](#setOverallocated-boolean-) | Overallocated가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setOvertimeCost(BigDecimal value)](#setOvertimeCost-java.math.BigDecimal-) | OvertimeCost의 값을 설정합니다. |
| [setOvertimeWork(Duration value)](#setOvertimeWork-com.aspose.tasks.Duration-) | OvertimeWork의 값을 설정합니다. |
| [setPeakUnits(double value)](#setPeakUnits-double-) | PeakUnits의 값을 설정합니다. |
| [setPercentWorkComplete(int value)](#setPercentWorkComplete-int-) | PercentWorkComplete의 값을 설정합니다. |
| [setRateScale(int value)](#setRateScale-int-) | RateScale 값을 설정합니다. |
| [setRegularWork(Duration value)](#setRegularWork-com.aspose.tasks.Duration-) | RegularWork의 값을 설정합니다. |
| [setRemainingCost(BigDecimal value)](#setRemainingCost-java.math.BigDecimal-) | RemainingCost의 값을 설정합니다. |
| [setRemainingOvertimeCost(BigDecimal value)](#setRemainingOvertimeCost-java.math.BigDecimal-) | RemainingOvertimeCost의 값을 설정합니다. |
| [setRemainingOvertimeWork(Duration value)](#setRemainingOvertimeWork-com.aspose.tasks.Duration-) | RemainingOvertimeWork의 값을 설정합니다. |
| [setRemainingWork(Duration value)](#setRemainingWork-com.aspose.tasks.Duration-) | RemainingWork의 값을 설정합니다. |
| [setResource(Resource value)](#setResource-com.aspose.tasks.Resource-) | 작업에 할당된 자원. |
| [setResponsePending(boolean value)](#setResponsePending-boolean-) | ResponsePending이 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setResume(Date value)](#setResume-java.util.Date-) | Resume 값을 설정합니다. |
| [setSV(double value)](#setSV-double-) | SV의 값을 설정합니다. |
| [setStart(Date value)](#setStart-java.util.Date-) | Start의 값을 설정합니다. |
| [setStartVariance(Duration value)](#setStartVariance-com.aspose.tasks.Duration-) | StartVariance 값을 설정합니다. |
| [setStop(Date value)](#setStop-java.util.Date-) | Stop 값을 설정합니다. |
| [setSummary(boolean value)](#setSummary-boolean-) | Summary가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setTask(Task value)](#setTask-com.aspose.tasks.Task-) | 리소스가 할당된 작업. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | 이 개체에 대해 `TimephasedData` 요소를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 설정합니다 (`TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 클래스). |
| [setUid(int value)](#setUid-int-) | Uid의 값을 설정합니다. |
| [setUnits(double value)](#setUnits-double-) | Units 값을 설정합니다. |
| [setUpdateNeeded(boolean value)](#setUpdateNeeded-boolean-) | UpdateNeeded가 설정되었는지 여부를 나타내는 값을 설정합니다. |
| [setVAC(double value)](#setVAC-double-) | VAC 값을 설정합니다. |
| [setWork(Duration value)](#setWork-com.aspose.tasks.Duration-) | Work의 값을 설정합니다. |
| [setWorkContour(int value)](#setWorkContour-int-) | WorkContour 값을 설정합니다. |
| [setWorkVariance(Duration value)](#setWorkVariance-com.aspose.tasks.Duration-) | WorkVariance의 값을 설정합니다. |
| [splitTask(Date start, Date finish, Calendar calendar)](#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-) | 작업을 두 부분으로 나눕니다. |
| [timephasedDataFromTaskDuration(Calendar calendar)](#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-) | 작업 기간 및 예정 시작 날짜를 기준으로 시간 단계 데이터 목록을 생성합니다. |
| [toString()](#toString--) | 인스턴스인 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스의 짧은 문자열 표현을 반환합니다. |
### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


이 컨테이너에서 속성이 매핑된 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키입니다. 속성 키를 가져오기 위한 [Asn](../../com.aspose.tasks/asn)입니다. |

**Returns:**
T - 이 컨테이너에서 속성이 매핑되는 값입니다.
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


지정된 속성을 이 컨테이너의 지정된 값에 매핑합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 지정된 속성 키입니다. 속성 키를 가져오기 위한 [Asn](../../com.aspose.tasks/asn)입니다. |
| val | T | 값입니다. |

### delete() {#delete--}
```
public final void delete()
```


프로젝트 할당 컬렉션에서 리소스 할당을 삭제합니다.

### equals(ResourceAssignment other) {#equals-com.aspose.tasks.ResourceAssignment-}
```
public final boolean equals(ResourceAssignment other)
```


이 인스턴스가 지정된 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스 인스턴스와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 이 인스턴스와 비교할 지정된 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스의 인스턴스입니다. |

**Returns:**
boolean - 지정된 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스 인스턴스가 이 인스턴스와 동일한 UID 값을 갖는 경우 **True**, 그렇지 않으면 **false**.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 객체입니다. |

**Returns:**
boolean - o가 이 인스턴스와 동일한 리소스와 작업을 할당하는 ResourceAssignment인 경우 **True**, 그렇지 않으면 **false**.
### getACWP() {#getACWP--}
```
public final double getACWP()
```


ACWP 값을 가져옵니다.

**Returns:**
double - ACWP 값입니다.
### getActualCost() {#getActualCost--}
```
public final BigDecimal getActualCost()
```


ActualCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - ActualCost 값입니다.
### getActualFinish() {#getActualFinish--}
```
public final Date getActualFinish()
```


ActualFinish 값을 가져옵니다.

**Returns:**
java.util.Date - ActualFinish 값입니다.
### getActualOvertimeCost() {#getActualOvertimeCost--}
```
public final BigDecimal getActualOvertimeCost()
```


ActualOvertimeCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - ActualOvertimeCost 값입니다.
### getActualOvertimeWork() {#getActualOvertimeWork--}
```
public final Duration getActualOvertimeWork()
```


ActualOvertimeWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWork.
### getActualOvertimeWorkProtected() {#getActualOvertimeWorkProtected--}
```
public final Duration getActualOvertimeWorkProtected()
```


ActualOvertimeWorkProtected 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualOvertimeWorkProtected.
### getActualStart() {#getActualStart--}
```
public final Date getActualStart()
```


ActualStart 값을 가져옵니다.

**Returns:**
java.util.Date - ActualStart 값입니다.
### getActualWork() {#getActualWork--}
```
public final Duration getActualWork()
```


ActualWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWork.
### getActualWorkProtected() {#getActualWorkProtected--}
```
public final Duration getActualWorkProtected()
```


ActualWorkProtected 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of ActualWorkProtected.
### getAssignmentOwner() {#getAssignmentOwner--}
```
public final String getAssignmentOwner()
```


AssignmentOwner 값을 가져옵니다.

**Returns:**
java.lang.String - AssignmentOwner 값입니다.
### getAssignmentOwnerGuid() {#getAssignmentOwnerGuid--}
```
public final String getAssignmentOwnerGuid()
```


AssignmentOwnerGuid 값을 가져옵니다.

**Returns:**
java.lang.String - AssignmentOwnerGuid 값입니다.
### getBCWP() {#getBCWP--}
```
public final double getBCWP()
```


BCWP 값을 가져옵니다.

**Returns:**
double - BCWP의 값.
### getBCWS() {#getBCWS--}
```
public final double getBCWS()
```


BCWS 값을 가져옵니다.

**Returns:**
double - BCWS의 값.
### getBaselines() {#getBaselines--}
```
public final AssignmentBaselineCollection getBaselines()
```


AssignmentBaselineCollection 객체를 가져옵니다. 할당과 연결된 기준값 컬렉션입니다.

**Returns:**
[AssignmentBaselineCollection](../../com.aspose.tasks/assignmentbaselinecollection) - AssignmentBaselineCollection object.
### getBookingType() {#getBookingType--}
```
public final int getBookingType()
```


BookingType 값을 가져옵니다.

**Returns:**
int - BookingType의 값.
### getBudgetCost() {#getBudgetCost--}
```
public final BigDecimal getBudgetCost()
```


BudgetCost 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - BudgetCost의 값.
### getBudgetWork() {#getBudgetWork--}
```
public final Duration getBudgetWork()
```


BudgetWork 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of BudgetWork.
### getCV() {#getCV--}
```
public final double getCV()
```


CV 값을 가져옵니다.

**Returns:**
double - CV의 값.
### getConfirmed() {#getConfirmed--}
```
public final boolean getConfirmed()
```


Confirmed가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Confirmed가 설정되었는지 여부를 나타내는 값입니다.
### getCost() {#getCost--}
```
public final BigDecimal getCost()
```


Cost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - Cost의 값.
### getCostRateTableType() {#getCostRateTableType--}
```
public final int getCostRateTableType()
```


CostRateTableType 값을 가져옵니다.

**Returns:**
int - CostRateTableType 값입니다.
### getCostVariance() {#getCostVariance--}
```
public final double getCostVariance()
```


CostVariance의 값을 가져옵니다.

**Returns:**
double - CostVariance의 값.
### getCreated() {#getCreated--}
```
public final Date getCreated()
```


Created의 값을 가져옵니다.

**Returns:**
java.util.Date - Created의 값.
### getDelay() {#getDelay--}
```
public final Duration getDelay()
```


Delay 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Delay.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeCollection getExtendedAttributes()
```


이 객체에 대한 ExtendedAttributeCollection 클래스의 인스턴스를 가져옵니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

**Returns:**
[ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) - an instance of the ExtendedAttributeCollection class for this object.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Finish의 값을 가져옵니다.

**Returns:**
java.util.Date - Finish의 값.
### getFinishVariance() {#getFinishVariance--}
```
public final Duration getFinishVariance()
```


FinishVariance 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of FinishVariance.
### getFixedMaterial() {#getFixedMaterial--}
```
public final boolean getFixedMaterial()
```


FixedMaterial이 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - FixedMaterial이 설정되었는지 여부를 나타내는 값입니다.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


이 할당에 대한 고유 식별자를 가져옵니다.

**Returns:**
java.util.UUID - 이 할당에 대한 고유 식별자입니다.
### getHyperlink() {#getHyperlink--}
```
public final String getHyperlink()
```


Hyperlink 값을 가져옵니다.

**Returns:**
java.lang.String - Hyperlink 값입니다.
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public final String getHyperlinkAddress()
```


HyperlinkAddress 값을 가져옵니다.

**Returns:**
java.lang.String - HyperlinkAddress 값입니다.
### getHyperlinkSubAddress() {#getHyperlinkSubAddress--}
```
public final String getHyperlinkSubAddress()
```


HyperlinkSubAddress 값을 가져옵니다.

**Returns:**
java.lang.String - HyperlinkSubAddress 값입니다.
### getItems() {#getItems--}
```
public final Iterable<IExtendedAttributeParent> getItems()
```


내부 사용을 위해 예약됨.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.IExtendedAttributeParent&gt; - \\{@inheritDoc\\}
### getLevelingDelay() {#getLevelingDelay--}
```
public final Duration getLevelingDelay()
```


LevelingDelay 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of LevelingDelay.
### getLinkedFields() {#getLinkedFields--}
```
public final boolean getLinkedFields()
```


LinkedFields가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - LinkedFields가 설정되었는지 여부를 나타내는 값입니다.
### getMilestone() {#getMilestone--}
```
public final boolean getMilestone()
```


Milestone이 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Milestone이 설정되었는지 여부를 나타내는 값입니다.
### getNotesRTF() {#getNotesRTF--}
```
public final String getNotesRTF()
```


RTF 형식의 텍스트 메모를 가져옵니다.

--------------------

MPP 형식에만 지원됩니다.

**Returns:**
java.lang.String - RTF 형식의 텍스트 노트입니다.
### getNotesText() {#getNotesText--}
```
public final String getNotesText()
```


RTF 데이터에서 추출된 메모의 일반 텍스트를 가져옵니다.

**Returns:**
java.lang.String - RTF 데이터에서 추출한 노트의 일반 텍스트입니다.
### getOverallocated() {#getOverallocated--}
```
public final boolean getOverallocated()
```


Overallocated가 설정되었는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Overallocated가 설정되었는지 여부를 나타내는 값입니다.
### getOvertimeCost() {#getOvertimeCost--}
```
public final BigDecimal getOvertimeCost()
```


OvertimeCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - OvertimeCost의 값.
### getOvertimeWork() {#getOvertimeWork--}
```
public final Duration getOvertimeWork()
```


OvertimeWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of OvertimeWork.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


이 할당에 대한 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent project for this assignment.
### getPeakUnits() {#getPeakUnits--}
```
public final double getPeakUnits()
```


PeakUnits의 값을 가져옵니다.

**Returns:**
double - PeakUnits의 값.
### getPercentWorkComplete() {#getPercentWorkComplete--}
```
public final int getPercentWorkComplete()
```


PercentWorkComplete의 값을 가져옵니다.

**Returns:**
int - PercentWorkComplete의 값.
### getRateScale() {#getRateScale--}
```
public final int getRateScale()
```


RateScale 값을 가져옵니다.

**Returns:**
int - RateScale 값입니다.
### getRegularWork() {#getRegularWork--}
```
public final Duration getRegularWork()
```


RegularWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RegularWork.
### getRemainingCost() {#getRemainingCost--}
```
public final BigDecimal getRemainingCost()
```


RemainingCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - RemainingCost의 값.
### getRemainingOvertimeCost() {#getRemainingOvertimeCost--}
```
public final BigDecimal getRemainingOvertimeCost()
```


RemainingOvertimeCost의 값을 가져옵니다.

**Returns:**
java.math.BigDecimal - RemainingOvertimeCost의 값.
### getRemainingOvertimeWork() {#getRemainingOvertimeWork--}
```
public final Duration getRemainingOvertimeWork()
```


RemainingOvertimeWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingOvertimeWork.
### getRemainingWork() {#getRemainingWork--}
```
public final Duration getRemainingWork()
```


RemainingWork의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of RemainingWork.
### getResource() {#getResource--}
```
public final Resource getResource()
```


작업에 할당된 자원.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - resource assigned to a task.
### getResponsePending() {#getResponsePending--}
```
public final boolean getResponsePending()
```


ResponsePending가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - ResponsePending이 설정되었는지 여부를 나타내는 값입니다.
### getResume() {#getResume--}
```
public final Date getResume()
```


Resume 값을 가져옵니다.

**Returns:**
java.util.Date - Resume의 값.
### getSV() {#getSV--}
```
public final double getSV()
```


SV의 값을 가져옵니다.

**Returns:**
double - SV의 값.
### getStart() {#getStart--}
```
public final Date getStart()
```


Start의 값을 가져옵니다.

**Returns:**
java.util.Date - Start의 값.
### getStartVariance() {#getStartVariance--}
```
public final Duration getStartVariance()
```


StartVariance 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of StartVariance.
### getStop() {#getStop--}
```
public final Date getStop()
```


Stop 값을 가져옵니다.

**Returns:**
java.util.Date - Stop의 값.
### getSummary() {#getSummary--}
```
public final boolean getSummary()
```


Summary가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - Summary가 설정되었는지 여부를 나타내는 값.
### getTask() {#getTask--}
```
public final Task getTask()
```


리소스가 할당된 작업.

**Returns:**
[Task](../../com.aspose.tasks/task) - task to which a resource is assigned.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


TimephasedData 요소(`TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)))를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 가져옵니다.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - the instance of [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) class containing elements of `TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) class.
### getTimephasedData(Date start, Date end) {#getTimephasedData-java.util.Date-java.util.Date-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end)
```


주어진 시작 및 종료 날짜의 [TimephasedDataType.AssignmentWork](../../com.aspose.tasks/timephaseddatatype\#AssignmentWork)에 해당하는 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/ [setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 인스턴스를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시간 구간 데이터의 시작 날짜. |
| 끝 | java.util.Date | 시간 구간 데이터의 종료 날짜. |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list containing instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedData(Date start, Date end, byte timephasedType) {#getTimephasedData-java.util.Date-java.util.Date-byte-}
```
public final TimephasedDataCollection getTimephasedData(Date start, Date end, byte timephasedType)
```


지정된 [TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)의 주어진 시작 및 종료 날짜 내에 `TimephasedData`([getTimephasedData()](../../com.aspose.tasks/resourceassignment\#getTimephasedData--)/[setTimephasedData(TimephasedDataCollection)](../../com.aspose.tasks/resourceassignment\#setTimephasedData-TimephasedDataCollection-)) 인스턴스를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 시간 구간 데이터의 시작 날짜. |
| 끝 | java.util.Date | 시간 구간 데이터의 종료 날짜. |
| timephasedType | byte | 시간 구간 데이터의 유형 ([TimephasedDataType](../../com.aspose.tasks/timephaseddatatype)). |

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - returns a list which contains instances of [TimephasedData](../../com.aspose.tasks/timephaseddata) class.
### getTimephasedWork(Date start, Date end) {#getTimephasedWork-java.util.Date-java.util.Date-}
```
public final double getTimephasedWork(Date start, Date end)
```


지정된 날짜 및 시간 간격에 대한 시간별 작업량을 가져옵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 날짜 시간 구간의 시작. |
| 끝 | java.util.Date | 날짜 시간 구간의 끝. |

**Returns:**
double - 지정된 날짜 시간 구간에 대한 시간별 작업량.
### getTimephasedWork(Date start, Date end, byte timephasedDataType) {#getTimephasedWork-java.util.Date-java.util.Date-byte-}
```
public final double getTimephasedWork(Date start, Date end, byte timephasedDataType)
```


지정된 날짜 및 시간 간격에 대한 시간별 작업량을 가져옵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 날짜 시간 구간의 시작. |
| 끝 | java.util.Date | 날짜 시간 구간의 끝. |
| timephasedDataType | 바이트 | 사용할 시간별 데이터 유형. |

**Returns:**
double - 지정된 날짜 시간 구간에 대한 시간별 작업량.
### getUid() {#getUid--}
```
public final int getUid()
```


Uid의 값을 가져옵니다.

**Returns:**
int - Uid의 값.
### getUnits() {#getUnits--}
```
public final double getUnits()
```


Units 값을 가져옵니다.

**Returns:**
double - Units의 값.
### getUpdateNeeded() {#getUpdateNeeded--}
```
public final boolean getUpdateNeeded()
```


UpdateNeeded가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - UpdateNeeded가 설정되었는지 여부를 나타내는 값.
### getVAC() {#getVAC--}
```
public final double getVAC()
```


VAC 값을 가져옵니다.

**Returns:**
double - VAC의 값.
### getWork() {#getWork--}
```
public final Duration getWork()
```


Work의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of Work.
### getWorkContour() {#getWorkContour--}
```
public final int getWorkContour()
```


WorkContour 값을 가져옵니다.

**Returns:**
int - WorkContour의 값.
### getWorkVariance() {#getWorkVariance--}
```
public final Duration getWorkVariance()
```


WorkVariance의 값을 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - a value of WorkVariance.
### hasChildren() {#hasChildren--}
```
public final boolean hasChildren()
```


이 리소스 할당에 하위 항목이 있음을 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항상 false.
### hasFixedRateUnits() {#hasFixedRateUnits--}
```
public final boolean hasFixedRateUnits()
```


HasFixedRateUnits가 설정되어 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - HasFixedRateUnits가 설정되었는지 여부를 나타내는 값.
### hashCode() {#hashCode--}
```
public int hashCode()
```


[ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### makeTPs(Date start, double time, Calendar calendar, List&lt;TimephasedData&gt; list, boolean isWorking, int type) {#makeTPs-java.util.Date-double-com.aspose.tasks.Calendar-java.util.List-com.aspose.tasks.TimephasedData--boolean-int-}
```
public final Date makeTPs(Date start, double time, Calendar calendar, List<TimephasedData> list, boolean isWorking, int type)
```


시간별 데이터 목록을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 지정된 시작 날짜. |
| time | double | 지정된 작업 시간. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 지정된 작업 캘린더. |
| list | java.util.List&lt;com.aspose.tasks.TimephasedData&gt; | 시간별 데이터 목록. |
| isWorking | boolean | 시간별 데이터가 작업 중인지 여부를 지정하는 플래그. |
| type | int | 지정된 시간별 데이터 유형. |

**Returns:**
java.util.Date - 목록에서 최대 날짜 또는 목록이 비어 있을 경우 시작 날짜.
### setACWP(double value) {#setACWP-double-}
```
public final void setACWP(double value)
```


ACWP의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | ACWP의 값. |

### setActualCost(BigDecimal value) {#setActualCost-java.math.BigDecimal-}
```
public final void setActualCost(BigDecimal value)
```


ActualCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | ActualCost의 값. |

### setActualFinish(Date value) {#setActualFinish-java.util.Date-}
```
public final void setActualFinish(Date value)
```


ActualFinish 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | ActualFinish의 값. |

### setActualOvertimeCost(BigDecimal value) {#setActualOvertimeCost-java.math.BigDecimal-}
```
public final void setActualOvertimeCost(BigDecimal value)
```


ActualOvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | ActualOvertimeCost의 값. |

### setActualOvertimeWork(Duration value) {#setActualOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWork(Duration value)
```


ActualOvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWork의 값. |

### setActualOvertimeWorkProtected(Duration value) {#setActualOvertimeWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualOvertimeWorkProtected(Duration value)
```


ActualOvertimeWorkProtected의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualOvertimeWorkProtected의 값. |

### setActualStart(Date value) {#setActualStart-java.util.Date-}
```
public final void setActualStart(Date value)
```


ActualStart 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | ActualStart의 값. |

### setActualWork(Duration value) {#setActualWork-com.aspose.tasks.Duration-}
```
public final void setActualWork(Duration value)
```


ActualWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWork의 값. |

### setActualWorkProtected(Duration value) {#setActualWorkProtected-com.aspose.tasks.Duration-}
```
public final void setActualWorkProtected(Duration value)
```


ActualWorkProtected의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | ActualWorkProtected의 값. |

### setAssignmentOwner(String value) {#setAssignmentOwner-java.lang.String-}
```
public final void setAssignmentOwner(String value)
```


AssignmentOwner의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | AssignmentOwner의 값. |

### setAssignmentOwnerGuid(String value) {#setAssignmentOwnerGuid-java.lang.String-}
```
public final void setAssignmentOwnerGuid(String value)
```


AssignmentOwnerGuid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | AssignmentOwnerGuid의 값. |

### setBCWP(double value) {#setBCWP-double-}
```
public final void setBCWP(double value)
```


BCWP의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | BCWP의 값. |

### setBCWS(double value) {#setBCWS-double-}
```
public final void setBCWS(double value)
```


BCWS의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | BCWS의 값. |

### setBookingType(int value) {#setBookingType-int-}
```
public final void setBookingType(int value)
```


BookingType의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | BookingType의 값. |

### setBudgetCost(BigDecimal value) {#setBudgetCost-java.math.BigDecimal-}
```
public final void setBudgetCost(BigDecimal value)
```


BudgetCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | BudgetCost의 값. |

### setBudgetWork(Duration value) {#setBudgetWork-com.aspose.tasks.Duration-}
```
public final void setBudgetWork(Duration value)
```


BudgetWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | BudgetWork의 값. |

### setCV(double value) {#setCV-double-}
```
public final void setCV(double value)
```


CV의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | CV의 값. |

### setConfirmed(boolean value) {#setConfirmed-boolean-}
```
public final void setConfirmed(boolean value)
```


Confirmed가 설정되어 있는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Confirmed가 설정되었는지 여부를 나타내는 값. |

### setCost(BigDecimal value) {#setCost-java.math.BigDecimal-}
```
public final void setCost(BigDecimal value)
```


Cost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | Cost의 값. |

### setCostRateTableType(int value) {#setCostRateTableType-int-}
```
public final void setCostRateTableType(int value)
```


CostRateTableType 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | CostRateTableType의 값. |

### setCostVariance(double value) {#setCostVariance-double-}
```
public final void setCostVariance(double value)
```


CostVariance의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | CostVariance의 값. |

### setCreated(Date value) {#setCreated-java.util.Date-}
```
public final void setCreated(Date value)
```


Created의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Created의 값. |

### setDelay(Duration value) {#setDelay-com.aspose.tasks.Duration-}
```
public final void setDelay(Duration value)
```


Delay 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Delay의 값. |

### setExtendedAttributes(ExtendedAttributeCollection value) {#setExtendedAttributes-com.aspose.tasks.ExtendedAttributeCollection-}
```
public final void setExtendedAttributes(ExtendedAttributeCollection value)
```


이 개체에 대해 ExtendedAttributeCollection 클래스의 인스턴스를 설정합니다.

--------------------

XML 형식에 대해서만 읽기가 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [ExtendedAttributeCollection](../../com.aspose.tasks/extendedattributecollection) | 이 객체에 대한 ExtendedAttributeCollection 클래스의 인스턴스. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Finish의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Finish의 값. |

### setFinishVariance(Duration value) {#setFinishVariance-com.aspose.tasks.Duration-}
```
public final void setFinishVariance(Duration value)
```


FinishVariance 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | FinishVariance의 값. |

### setFixedMaterial(boolean value) {#setFixedMaterial-boolean-}
```
public final void setFixedMaterial(boolean value)
```


FixedMaterial이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | FixedMaterial이 설정되었는지 여부를 나타내는 값. |

### setFixedRateUnits(boolean value) {#setFixedRateUnits-boolean-}
```
public final void setFixedRateUnits(boolean value)
```


HasFixedRateUnits가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | HasFixedRateUnits가 설정되었는지 여부를 나타내는 값. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


이 할당에 대한 고유 식별자를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.UUID | 이 할당에 대한 고유 식별자. |

### setHyperlink(String value) {#setHyperlink-java.lang.String-}
```
public final void setHyperlink(String value)
```


Hyperlink 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Hyperlink의 값. |

### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public final void setHyperlinkAddress(String value)
```


HyperlinkAddress 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | HyperlinkAddress의 값. |

### setHyperlinkSubAddress(String value) {#setHyperlinkSubAddress-java.lang.String-}
```
public final void setHyperlinkSubAddress(String value)
```


HyperlinkSubAddress 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | HyperlinkSubAddress의 값. |

### setLevelingDelay(Duration value) {#setLevelingDelay-com.aspose.tasks.Duration-}
```
public final void setLevelingDelay(Duration value)
```


LevelingDelay 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | LevelingDelay의 값. |

### setLinkedFields(boolean value) {#setLinkedFields-boolean-}
```
public final void setLinkedFields(boolean value)
```


LinkedFields가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | LinkedFields가 설정되었는지 여부를 나타내는 값. |

### setMaterialResourceUnits(double units, int rateScaleType) {#setMaterialResourceUnits-double-int-}
```
public final void setMaterialResourceUnits(double units, int rateScaleType)
```


가변 재료 소비가 있는 물자 리소스 할당에 대한 단위를 설정합니다. 가변 재료 소비란 할당 기간이 변경됨에 따라 사용되는 재료의 양이 비례적으로 변함을 의미합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 단위 | double | 해당 기간에 누적된 단위 수. |
|  | rateScaleType | int | 단위 값이 누적되는 기간. |

--------------------

예를 들어, '123/월'을 설정하려면 SetUnitsScaled(123D, RateScaleType.Month)를 호출해야 합니다. |

### setMilestone(boolean value) {#setMilestone-boolean-}
```
public final void setMilestone(boolean value)
```


Milestone이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Milestone이 설정되었는지 여부를 나타내는 값. |

### setNotesRTF(String value) {#setNotesRTF-java.lang.String-}
```
public final void setNotesRTF(String value)
```


RTF 형식으로 텍스트 메모를 설정합니다.

--------------------

MPP 형식에만 지원됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | RTF 형식의 텍스트 메모. |

### setNotesText(String value) {#setNotesText-java.lang.String-}
```
public final void setNotesText(String value)
```


RTF 데이터에서 추출한 메모의 일반 텍스트를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | RTF 데이터에서 추출한 메모의 일반 텍스트. |

### setOverallocated(boolean value) {#setOverallocated-boolean-}
```
public final void setOverallocated(boolean value)
```


Overallocated가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Overallocated가 설정되었는지 여부를 나타내는 값. |

### setOvertimeCost(BigDecimal value) {#setOvertimeCost-java.math.BigDecimal-}
```
public final void setOvertimeCost(BigDecimal value)
```


OvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | OvertimeCost 값. |

### setOvertimeWork(Duration value) {#setOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setOvertimeWork(Duration value)
```


OvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | OvertimeWork 값. |

### setPeakUnits(double value) {#setPeakUnits-double-}
```
public final void setPeakUnits(double value)
```


PeakUnits의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | PeakUnits 값. |

### setPercentWorkComplete(int value) {#setPercentWorkComplete-int-}
```
public final void setPercentWorkComplete(int value)
```


PercentWorkComplete의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | PercentWorkComplete 값. |

### setRateScale(int value) {#setRateScale-int-}
```
public final void setRateScale(int value)
```


RateScale 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | RateScale의 값. |

### setRegularWork(Duration value) {#setRegularWork-com.aspose.tasks.Duration-}
```
public final void setRegularWork(Duration value)
```


RegularWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RegularWork 값. |

### setRemainingCost(BigDecimal value) {#setRemainingCost-java.math.BigDecimal-}
```
public final void setRemainingCost(BigDecimal value)
```


RemainingCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | RemainingCost 값. |

### setRemainingOvertimeCost(BigDecimal value) {#setRemainingOvertimeCost-java.math.BigDecimal-}
```
public final void setRemainingOvertimeCost(BigDecimal value)
```


RemainingOvertimeCost의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | RemainingOvertimeCost 값. |

### setRemainingOvertimeWork(Duration value) {#setRemainingOvertimeWork-com.aspose.tasks.Duration-}
```
public final void setRemainingOvertimeWork(Duration value)
```


RemainingOvertimeWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingOvertimeWork 값. |

### setRemainingWork(Duration value) {#setRemainingWork-com.aspose.tasks.Duration-}
```
public final void setRemainingWork(Duration value)
```


RemainingWork의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | RemainingWork 값. |

### setResource(Resource value) {#setResource-com.aspose.tasks.Resource-}
```
public final void setResource(Resource value)
```


작업에 할당된 자원.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Resource](../../com.aspose.tasks/resource) | 작업에 할당된 리소스. |

### setResponsePending(boolean value) {#setResponsePending-boolean-}
```
public final void setResponsePending(boolean value)
```


ResponsePending이 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | ResponsePending가 설정되었는지 여부를 나타내는 값. |

### setResume(Date value) {#setResume-java.util.Date-}
```
public final void setResume(Date value)
```


Resume 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Resume 값. |

### setSV(double value) {#setSV-double-}
```
public final void setSV(double value)
```


SV의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | SV 값. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Start의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Start의 값. |

### setStartVariance(Duration value) {#setStartVariance-com.aspose.tasks.Duration-}
```
public final void setStartVariance(Duration value)
```


StartVariance 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | StartVariance 값. |

### setStop(Date value) {#setStop-java.util.Date-}
```
public final void setStop(Date value)
```


Stop 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Stop 값. |

### setSummary(boolean value) {#setSummary-boolean-}
```
public final void setSummary(boolean value)
```


Summary가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | Summary가 설정되었는지 여부를 나타내는 값. |

### setTask(Task value) {#setTask-com.aspose.tasks.Task-}
```
public final void setTask(Task value)
```


리소스가 할당된 작업.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | 리소스가 할당된 작업. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


이 개체에 대해 `TimephasedData` 요소를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스를 설정합니다 (`TimephasedData`([getTimephasedData](../../com.aspose.tasks/resourceassignment\\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 클래스).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | 요소 `TimephasedData`를 포함하는 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스의 인스턴스([getTimephasedData](../../com.aspose.tasks/resourceassignment\#getTimephasedData-java.util.Date-java.util.Date-byte-)/[setTimephasedData](../../com.aspose.tasks/resourceassignment\#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-)) 클래스. |

### setUid(int value) {#setUid-int-}
```
public final void setUid(int value)
```


Uid의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Uid의 값. |

### setUnits(double value) {#setUnits-double-}
```
public final void setUnits(double value)
```


Units 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | Units 값. |

### setUpdateNeeded(boolean value) {#setUpdateNeeded-boolean-}
```
public final void setUpdateNeeded(boolean value)
```


UpdateNeeded가 설정되었는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | UpdateNeeded가 설정되었는지 여부를 나타내는 값. |

### setVAC(double value) {#setVAC-double-}
```
public final void setVAC(double value)
```


VAC 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | double | VAC 값. |

### setWork(Duration value) {#setWork-com.aspose.tasks.Duration-}
```
public final void setWork(Duration value)
```


Work의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Work의 값. |

### setWorkContour(int value) {#setWorkContour-int-}
```
public final void setWorkContour(int value)
```


WorkContour 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | WorkContour 값. |

### setWorkVariance(Duration value) {#setWorkVariance-com.aspose.tasks.Duration-}
```
public final void setWorkVariance(Duration value)
```


WorkVariance의 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | WorkVariance의 값. |

### splitTask(Date start, Date finish, Calendar calendar) {#splitTask-java.util.Date-java.util.Date-com.aspose.tasks.Calendar-}
```
public final void splitTask(Date start, Date finish, Calendar calendar)
```


작업을 두 부분으로 나눕니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 시작 | java.util.Date | 분할 기준이 되는 작업 중단의 시작. |
| 완료 | java.util.Date | 분할 기준이 되는 작업 중단의 끝. |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 분할 기준이 되는 캘린더. |

### timephasedDataFromTaskDuration(Calendar calendar) {#timephasedDataFromTaskDuration-com.aspose.tasks.Calendar-}
```
public final void timephasedDataFromTaskDuration(Calendar calendar)
```


작업 기간 및 예정 시작 날짜를 기준으로 시간 단계 데이터 목록을 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| calendar | [Calendar](../../com.aspose.tasks/calendar) | 시간 단계 데이터를 생성할 캘린더. |

### toString() {#toString--}
```
public String toString()
```


인스턴스 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 클래스의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다.

**Returns:**
java.lang.String - 할당 객체를 나타내는 짧은 문자열.
